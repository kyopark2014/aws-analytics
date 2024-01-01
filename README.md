# AWS Analytics

## Analytics Basic

### 파일시스템

- HDFS (Hadoop Distributed File System)
 -- 순차접근(Sequential Access) 방식을 통해 불편 데이터를 저장하는 데 최적화 되어 있음
* 데이터를 block 으로 나누어 저장, 128MB (기본)
* 여러대의 서버에 replica를 만들어서 resilience(회복성)을 제공
- Amazon S3: 클라우드 스토리지
- Azure Data Lake Store: 클라우드 스토리지
- Apache Kudu: IoT 환경에서 데이터 분석

### 데이터 분석 엔진/프레임워크

- MapReduce
- Apache Spark: 스트림 처리와 머신러닝 워크로드
- Apache Impala
- Apache Hive: SQL Engine

### 데이터 분석 아키텍처의 특징

- 대용량
- 분산
- 무공유 (Shared nothing)

## AWS Glue

AWS Glue  is a serverless data integration service that makes it easy to discover, prepare, and combine data for analytics, machine learning, and application development. AWS Glue provides all the capabilities needed for data integration so that you can start analyzing your data and put it to use in minutes instead of months.


AWS Glue는 분석, 기계 학습 및 애플리케이션 개발을 위해 데이터를 쉽게 탐색, 준비, 그리고 조합할 수 있도록 지원하는 서버리스 데이터 통합 서비스입니다. AWS Glue에서는 데이터 통합에 필요한 모든 기능을 제공하므로, 몇 개월이 아니라 몇 분 안에 데이터 분석을 시작하고 해당 내용을 활용할 수 있습니다.

데이터 통합은 분석, 기계 학습 및 애플리케이션 개발을 위해 데이터를 준비하고 결합하는 프로세스입니다. 이 작업은 다양한 소스에서 데이터 검색 및 추출, 데이터 강화, 정리, 정규화 및 결합, 데이터베이스, 데이터 웨어하우스 및 데이터 레이크(Data Lake)에 데이터 로드 및 구성 등의 여러 작업을 포함합니다. 이러한 작업은 종종 각자 다른 제품을 사용하는 다른 유형의 사용자가 취급합니다.

AWS Glue는 데이터 통합을 쉽게 준비할 수 있도록 시각적 인터페이스와 코드 기반 인터페이스를 모두 제공합니다. 사용자는 AWS Glue 데이터 카탈로그를 사용하여 데이터를 쉽게 찾고 액세스할 수 있습니다. 데이터 엔지니어와 ETL (추출, 변형 및 로드) 개발자는 AWS Glue Studio에서 몇 번의 클릭으로 ETL 워크플로를 시각적으로 생성, 실행 및 모니터링할 수 있습니다. 데이터 분석가와 데이터 사이언티스트는 [AWS Glue DataBrew](https://aws.amazon.com/ko/glue/features/databrew/)를 사용하여 코드를 작성하지 않고도 데이터를 시각적으로 정리하고 정규화할 수 있습니다. [AWS Glue Elastic Views](https://aws.amazon.com/ko/glue/features/elastic-views/)를 통해 애플리케이션 개발자는 익숙한 Structured Query Language (SQL)를 사용하여 다른 데이터 저장소 간의 데이터를 조합 및 복제할 수 있습니다


데이터 분석 또는 Machine Learning에 을 위한 데이터 준비를 위해, 데이터 scientist나 Analysts는 data를 cleaning 하거나 normaliza 하는 작업을 수행하여야 합니다. 이러한 과정은 수주 또는 수개월을 수행하기도 하는데, 80% 시간을 이런 데이터의 data perperation task을 위해 사용하고 있다고 합니다. 이를 위해 clean, combine, pivot, transpose 하는 작업을 Glue가 지원합니다. 


## 처리하는 작업 

- Clean
- Transform
- Concatenate
- Covert to better formats
- Schedule transformations
- Event-driven transformations

## Workshop

[Glue Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/aaaabcab-5e1e-4bff-b604-781a804763e1/en-US)


## Reference 

[AWS Glue - 간단하고 확장 가능한 서버리스 데이터 통합](https://aws.amazon.com/ko/glue/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc)


[Introducing AWS Glue DataBrew](https://youtu.be/oAxvd547kMU)


[Working with AWS Glue Studio - Part 1](https://www.youtube.com/watch?v=KkN8lQ-jr58)

[Working with AWS Glue Studio - Part 2](https://www.youtube.com/watch?v=pnWdkKl2hZw)
 
[Working with AWS Glue Studio - Part3](https://www.youtube.com/watch?v=o7ZoigUcu1M)

