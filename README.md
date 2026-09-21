# 📝[2026년 한이음 드림업 공모전 GitHub README 템플릿]
- 이 파일은 2026년 한이음 드림업 프로젝트를 수행하는 학생들에게 README 작성의 가이드라인을 제공하기 위해 제작되었습니다.
- [Git & Github 기초사용법 알아보기](https://github.com/hanium-dreamup-challenge/git_guide/blob/main/README_git_guide.md)
---
## **💡README 작성방법**
- 프로젝트에서 사용되는 소스코드를 레포지토리에 업로드 한 후, 아래 가이드에 따라 README.md파일을 작성해주세요.
- 필수 작성 항목(5가지) : 프로젝트 개요, 팀원 소개, 시스템 구성도, 작품 소개영상, 핵심 소스코드 
- 프로젝트 저장소명 규칙 : `https://github.com/깃허브계정명/프로젝트 번호`
- 예시) 깃허브 계정이 hanium이고, 프로젝트 번호가 26_HC001일 경우 -> `https://github.com/hanium/25_HC001`
- 아래 항목 및 내용은 이해를 돕기위한 예시입니다. 참고만 하되 자유롭게 추가 및 작성해주시기 바랍니다.

---

## **💡1. 프로젝트 개요**

**1-1. 프로젝트 소개**
- 프로젝트 명 : 한이음 드림업 AI검색 서비스
- 프로젝트 정의 : 사용자의 검색 의도를 이해하고 최적의 정보를 제공하는 AI 기반 맞춤형 검색 서비스
  <img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/b25d0039-dfc8-4a6f-85c0-567a92e4039f" /></br>

**1-2. 개발 배경 및 필요성**
- 현대 사회는 방대한 정보가 실시간으로 생성되고 축적되고 있습니다. 그러나 사용자가 원하는 정확한 정보를 찾기 위해서는 여전히 많은 시간과 노력이 필요합니다. 기존 키워드 기반 검색 방식은 사용자의 맥락이나 의도를 충분히 반영하지 못해 효율성이 떨어집니다. 따라서 사용자의 검색 목적을 인공지능이 이해하고 개인화된 결과를 제공하는 맞춤형 검색 서비스가 필요합니다.

**1-3. 프로젝트 특장점**
- 사용자의 검색 의도와 맥락을 이해하는 자연어 이해 기반 검색 서비스
- 단순 키워드 매칭이 아닌 의미 기반 정보 추천 및 순위화
- 개인별 기록과 관심사를 반영한 맞춤형 검색 결과 제공
- 다양한 데이터 소스를 연동해 멀티도메인 활용 가능성 확보
- 최신 AI/ML 프레임워크와 대규모 언어모델(LLM)을 활용한 최적화된 사용자 경험

**1-4. 주요 기능**
- AI 맞춤 검색 서비스 : 검색 의도를 분석하고 개인화된 결과 제공
- 자연어 질의 처리 : 키워드뿐 아니라 문장 단위 질문도 이해 가능
- 의미 기반 추천 : 단순한 ‘정확 단어 일치’가 아닌 맥락과 의미를 기반으로 한 결과 제공
- 맞춤형 필터링 및 정렬 : 사용자 성향에 따라 검색 결과 필터 및 순위 조정
- 멀티플랫폼 지원 : 웹·모바일 등 다양한 기기 환경에서 최적화된 검색 경험 제공

**1-5. 기대 효과 및 활용 분야**
- 기대 효과 : 검색 품질 향상 및 정보 탐색 효율 극대화, 다양한 산업 분야에서 데이터 활용성 확대
- 활용 분야 : 학술·연구, 커머스·쇼핑, 헬스케어, 뉴스·미디어, 기업 내부 문서 검색 등

**1-6. 기술 스택**
- 프론트엔드 : React, Next.js, Tailwind CSS
- 백엔드 : Python(FastAPI), Node.js, Django
- AI/ML : PyTorch, TensorFlow, Hugging Face, OpenAI API
- 데이터베이스 : PostgreSQL, MongoDB, Elasticsearch
- 클라우드 : AWS
- 배포 및 관리 : Docker, Kubernetes, GitHub Actions

---

## **💡2. 팀원 소개(이름 기재X)**

| <img width="80" height="100" src="https://github.com/user-attachments/assets/ab73bb1c-c1d4-464d-8ad3-635b45d5a8ae" > | <img width="80" height="100" alt="image" src="https://github.com/user-attachments/assets/c7f66b7c-ab84-41fa-8fba-b49dba28b677" > | <img width="80" height="100" alt="image" src="https://github.com/user-attachments/assets/c33252c7-3bf6-43cf-beaa-a9e2d9bd090b" > | <img width="80" height="100" alt="image" src="https://github.com/user-attachments/assets/0d5909f0-fc73-4ab9-be09-4d48e3e71083" > | <img width="80" height="100" alt="image" src="https://github.com/user-attachments/assets/c7f66b7c-ab84-41fa-8fba-b49dba28b677" > |
|:---:|:---:|:---:|:---:|:---:|
| **멘티1** | **멘티2** | **멘티3** | **멘티4** | **멘토** |
| • 개발총괄 <br> • UI/UX 기획 | • 백엔드 <br> • 프론트엔드 | • API 개발 <br> • DB 서버 구축 |• 데이터 분석 <br> • 전처리 | • 프로젝트 멘토 <br> • 기술 자문 |



---
## **💡3. 시스템 구성도**
> **(참고)** S/W구성도, H/W구성도, 서비스 흐름도 등을 작성합니다. 시스템의 동작 과정 등을 추가할 수도 있습니다.
- 서비스 구성도
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/28fc8453-d1a0-4184-8fd0-130d93d18545" />


- 엔티티 관계도
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/76e3347b-6d94-491e-8aeb-a7b4601c54d5" />


---
## **💡4. 작품 소개영상**
> **참고**: 썸네일과 유튜브 영상을 등록하는 방법입니다.
```Python
아래와 같이 작성하면, 썸네일과 링크등록을 할 수 있습니다.
[![영상 제목](유튜브 썸네일 URL)](유튜브 영상 URL)

작성 예시 : 저는 다음과 같이 작성하니, 아래와 같이 링크가 연결된 썸네일 이미지가 등록되었네요! 
[![한이음 드림업 프로젝트 소개](https://github.com/user-attachments/assets/16435f88-e7d3-4e45-a128-3d32648d2d84)](https://youtu.be/YcD3Lbn2FRI?si=isERqIAT9Aqvdqwp)
```
[![한이음 드림업 프로젝트 소개](https://github.com/user-attachments/assets/16435f88-e7d3-4e45-a128-3d32648d2d84)](https://youtu.be/YcD3Lbn2FRI?si=isERqIAT9Aqvdqwp)


---
## **💡5. 핵심 소스코드**
- 소스코드 설명 : API를 활용해서 자동 배포를 생성하는 메서드입니다.

```Java
    private static void start_deployment(JsonObject jsonObject) {
        String user = jsonObject.get("user").getAsJsonObject().get("login").getAsString();
        Map<String, String> map = new HashMap<>();
        map.put("environment", "QA");
        map.put("deploy_user", user);
        Gson gson = new Gson();
        String payload = gson.toJson(map);

        try {
            GitHub gitHub = GitHubBuilder.fromEnvironment().build();
            GHRepository repository = gitHub.getRepository(
                    jsonObject.get("head").getAsJsonObject()
                            .get("repo").getAsJsonObject()
                            .get("full_name").getAsString());
            GHDeployment deployment =
                    new GHDeploymentBuilder(
                            repository,
                            jsonObject.get("head").getAsJsonObject().get("sha").getAsString()
                    ).description("Auto Deploy after merge").payload(payload).autoMerge(false).create();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
```
