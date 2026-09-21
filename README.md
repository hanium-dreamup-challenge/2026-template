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

**1-2. 개발 배경 및 필요성**

**1-3. 프로젝트 특장점**

**1-4. 주요 기능**

**1-5. 기대 효과 및 활용 분야**

**1-6. 기술 스택**

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
