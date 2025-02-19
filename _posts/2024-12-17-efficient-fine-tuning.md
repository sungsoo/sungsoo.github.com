---
layout: post
title:  Efficient Fine-tuning LLMs with PEFT and LoRA
date: 2024-12-17
categories: [artificial intelligence]
tags: [machine learning]

---

# Efficient Fine-tuning

# 효율적인 미세 조정: 사전 학습된 대규모 모델의 잠재력을 극대화하는 방법

사전 학습된 대규모 모델은 방대한 양의 지식을 내재하고 있어 적은 양의 데이터로도 우수한 성능을 발휘할 수 있습니다. 하지만 이러한 모델을 미세 조정하는 데에는 많은 비용과 시간이 소요됩니다. 효율적인 미세 조정은 이러한 비용을 최소화하면서 성능을 극대화하는 것을 목표로 합니다.

## 파라미터 효율적인 미세 조정(PEFT) 기술

최근에는 파라미터 효율적인 미세 조정(PEFT) 기술이 주목받고 있습니다. PEFT는 기존 모델의 파라미터를 모두 수정하는 대신, 일부 파라미터만 조정하여 계산량을 줄이고, 더 빠르게 학습할 수 있도록 해줍니다.

* **LoRA:** 가장 인기 있는 PEFT 방법 중 하나로, 모델의 가중치 행렬에 저랭크 분해를 적용하여 학습 가능한 행렬을 추가합니다. 이를 통해 소수의 파라미터만으로도 모델을 효과적으로 미세 조정할 수 있습니다.
* **LLaMA-Adapter:** LLaMA 모델을 지시 따르기 모델로 효율적으로 미세 조정하는 방법입니다. 컨텍스트에 학습 가능한 어댑테이션 프롬프트를 추가하고, 제로 초기화된 어텐션 메커니즘을 학습하여 적은 계산량으로 높은 성능을 달성합니다.
* **IA³:** LoRA와 유사하게 모델의 활성화 값에 학습 가능한 벡터를 곱하여 모델을 조정합니다.
* **Soft Prompting:** 입력 임베딩에 학습 가능한 파라미터를 추가하여 모델의 출력을 조절하는 방법입니다.
* **Adapters:** 어텐션 블록 내부에 학습 가능한 파라미터를 추가하여 모델을 조정합니다.
* **Prefix Tuning:** 어텐션의 KV 표현에 학습 가능한 벡터를 추가하여 모델을 조정합니다.
* **LayerNorm Tuning:** 모델의 LayerNorm 레이어를 미세 조정하는 방법으로, 예상외로 좋은 성능을 보여줍니다.
* **GaLoRA:** LoRA를 모델의 그래디언트에 적용하는 방법입니다.
* **REFT:** 소스 모델 파라미터와 최적화 목표 사이에 선형 프로빙 전략을 적용하는 방법입니다.

## PEFT 기술의 장점

* **빠른 학습:** 기존 모델의 대부분을 고정하고 일부 파라미터만 학습하기 때문에 학습 시간이 단축됩니다.
* **낮은 계산 비용:** 적은 수의 파라미터만 학습하기 때문에 메모리 사용량과 연산량이 줄어듭니다.
* **높은 성능:** 기존 모델의 성능을 유지하면서 새로운 태스크에 대한 적응력을 높일 수 있습니다.

## 결론

PEFT 기술은 사전 학습된 대규모 모델을 효율적으로 활용하기 위한 중요한 방법입니다. 다양한 PEFT 기술들이 개발되고 있으며, 앞으로 더욱 발전하여 더욱 효율적이고 강력한 모델을 만드는 데 기여할 것으로 기대됩니다.

**핵심 키워드:** 파라미터 효율적인 미세 조정, PEFT, LoRA, LLaMA-Adapter, Soft Prompting, Adapters, Prefix Tuning, LayerNorm Tuning, GaLoRA, REFT, 사전 학습 모델, 미세 조정

## LoRA & QLoRA Fine-tuning Explained In-Depth

In this video, I dive into how LoRA works vs full-parameter fine-tuning, explain why QLoRA is a step up, and provide an in-depth look at the LoRA-specific hyperparameters: Rank, Alpha, and Dropout.

<iframe width="600" height="400" src="https://www.youtube.com/embed/t1caDsMzWBk?si=ZPgC78SAEx2yxVJe" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Fine-tuning LLMs with PEFT and LoRA

<iframe width="600" height="400" src="https://www.youtube.com/embed/Us5ZFp16PaU?si=zbp-4aGA3KqBDwDw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

# 분산화와 학습 역학

## 분산화: 클라우드를 넘어

많은 모델들이 단일 장치가 아닌 분산된 하드웨어 환경에서 학습 및 추론을 수행하도록 설계되고 있습니다. 하지만 지리적으로 분산된 클러스터에서는 통신 오버헤드가 발생하여 성능 저하를 야기할 수 있습니다. 이러한 문제를 해결하기 위해 다양한 연구가 진행되고 있습니다.

* **CacheGen:** KV 캐시를 압축하여 통신 비용을 줄이는 방법입니다.
* **CocktailSGD:** 스파시파이와 양자화 기법을 결합하여 대규모 모델을 느린 네트워크 환경에서도 학습할 수 있도록 합니다.
* **DiLoCo:** 연결이 제한적인 환경에서도 효율적인 연합 학습 알고리즘을 제안합니다.
* **Petals:** 개인 사용자의 GPU를 활용하여 대규모 모델을 학습하고 서비스하는 시스템입니다.

분산 학습은 다양한 장점을 제공합니다. 이종 장치를 연결하고, 장애 허용성을 높이며, 네트워크 대역폭을 최적화하고, 데이터 프라이버시를 보장할 수 있습니다.

## 학습 역학: 거대한 언어 모델의 신비를 풀다

거대한 언어 모델의 학습 과정은 매우 복잡하고 아직 완전히 이해되지 않았습니다. 모델의 크기가 커질수록 학습 역학은 더욱 복잡해지며, 모델의 성능에 영향을 미치는 다양한 요소들이 존재합니다. 

* **중간 체크포인트 분석:** 모델 학습 과정에서 중간 체크포인트를 분석하여 모델의 성능 변화를 추적하고, 모델의 특성을 파악할 수 있습니다.
* **메모리 능력 분석:** 모델이 학습 데이터를 얼마나 잘 기억하고 있는지 분석하여 모델의 일반화 능력을 이해할 수 있습니다.
* **Pythia:** 다양한 크기의 모델을 공개하여 연구자들이 모델 학습 과정을 더 쉽게 연구할 수 있도록 지원합니다.
* **OLMO:** 모델 학습에 사용된 데이터, 코드 등을 공개하여 학습 과정을 투명하게 만들고 연구를 촉진합니다.

## 결론

분산 학습과 모델 학습 역학에 대한 연구는 거대한 언어 모델의 발전을 위한 필수적인 요소입니다. 이러한 연구를 통해 우리는 더욱 효율적이고 강력한 AI 모델을 개발할 수 있을 것입니다.

**핵심 키워드:** 분산 학습, 거대 언어 모델, 학습 역학, CacheGen, CocktailSGD, DiLoCo, Petals, Pythia, OLMO

