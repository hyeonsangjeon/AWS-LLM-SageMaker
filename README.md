# AWS-LLM-SageMaker

개발자와 솔루션 빌더를 대상으로 하는 이 실습 워크샵에서는 [Amazon SageMaker](https://aws.amazon.com/sagemaker/)을 통해 파운데이션 모델(FM)을 활용하는 방법을 소개합니다.

이 실습에서는 Generative AI에 대해 고객들이 가장 많이 사용하는 몇 가지 사용 패턴 GenAI를 이용하여 생산성을 향상시킴으로써 조직의 가치를 창출하는 기술의 예제를 보여줍니다.  
이는 이메일 작성, 텍스트 요약, 질문에 대한 답변, 챗봇 구축, 이미지 생성에 도움이 되는 기초 모델을 활용하여 달성할 수 있습니다.


### AWS Samples Github 배포 실습 자료 안내

본 실습 자료는 AWS Samples Github에 배포됩니다. 현재 실습 자료는 AWS Samples 공식 자료보다 항상 최신 선반영됩니다.

#### LLM - RAG: Opensearch with SageMaker Endpoint LLM Polyglot
- 토픽: LLM - RAG: Opensearch with SageMaker Endpoint LLM Polyglot
- 반영 링크: https://github.com/aws-samples/aws-ai-ml-workshop-kr/tree/master/genai/aws-gen-ai-kr/20_applications/04_rag_finance_opensearch_sllm_workshop
- 최근 반영일: 2024.04.25

#### [Tuner] QLoRA fine-tuning
- 토픽: [Tuner] QLoRA fine-tuning
- 반영 링크: https://github.com/aws-samples/aws-ai-ml-workshop-kr/tree/master/genai/aws-gen-ai-kr/30_fine_tune/01-instruction-tuning-peft-qlora
- 최근 반영일: 2024.04.18

## LLM - RAG : Opensearch with SageMaker Endpoint LLM Ployglot
1. [Amazon SageMaker와 Amazon Opensearch로 RAG (Retrieval-Augmented Generation) 구현실습 ](https://github.com/hyeonsangjeon/AWS-LLM-SageMaker/tree/main/RAG-SageMaker/rag-fsi-data-workshop) -
   RAG (Retrieval-Augmented Generation)는 정보 검색과 텍스트 생성을 결합한 혁신적인 NLP 아키텍처입니다. 이번 실습에서는 RAG가 어떻게 Amazon Opensearch와 통합되어 외부의 신뢰할 수 있는 데이터베이스나 문서를 검색하는 과정을 강화하는지 간단한 실습을 통해 알아봅니다.
   이 실습에서는 SageMaker Endpoint와 Amazon Openssearch에서 Embedding 데이터 입력, SDK, 그리고 [LangChain](https://python.langchain.com/docs/get_started/introduction) 및 [FAISS](https://faiss.ai/index.html)와 같은 오픈소스 소프트웨어를 통해 이러한 패턴을 구현하는 실무 경험을 쌓을 수 있습니다.




## [Tuner] QLoRA fine-tuning
- [KULLM-Polyglot-12.8B](PEFT)

### Filenames
- `1_prepare-dataset-alpaca-method.ipynb`: instruction 데이터 세트로부터 훈련 데이터 세트를 준비합니다. 각 샘플을 토크나이즈하는 방식입니다.
- `1_prepare-dataset-chunk-method.ipynb`: instruction 데이터 세트로부터 훈련 데이터 세트를 준비합니다. 샘플을 모두 모아서(concatenate) 청크 크기(chunk size)만큼 분할하는 방식입니다.
- `2_local-train-debug-lora.ipynb`: 본격적으로 훈련 인스턴스에서 수행하기 전에 개발 환경에서 일부 샘플 데이터로 디버그를 수행합니다. 이미 파인 튜닝에 익숙한 분들은 이 핸즈온을 건너뛰고 3_sm-train-lora.ipynb을 진행해 주세요.
- `3_sm-train-lora.ipynb`: SageMaker 훈련 인스턴스에서 파인튜닝을 수행합니다. 

