
본 API 시스템은 제조 공정의 수율 향상 및 불량률 최소화를 위한 **지능형 품질 검사(Intelligent Quality Inspection)** 백엔드 서비스입니다. 
산업경영공학의 통계적 품질 관리(SQC) 기법과 딥러닝 기반 컴퓨터 비전 기술을 융합하여 실시간으로 부품의 결함을 탐지합니다.

### 💡 주요 기능
- **실시간 결함 탐지 (Real-time Defect Detection):** 업로드된 부품 이미지를 분석하여 불량 여부, 결함 유형(스크래치, 파손, 오염 등), 모델의 신뢰도(Confidence Score)를 즉각적으로 파악합니다.
- **후속 조치 자동 분류 (Decision Support):** 탐지된 결함 종류와 신뢰도를 기반으로 공정 내 후속 조치(통과, 재검사, 폐기 등)를 시스템이 제안합니다.

### 🏗 시스템 아키텍처
- **Framework:** FastAPI (비동기 처리 기반 고성능 API 제공 및 자동 Swagger UI 생성)
- **Deployment:** Docker & MLOps Pipeline (GitHub Actions 기반의 CI/CD 파이프라인 구축)
- **Model Mock-up:** 향후 PyTorch/TensorFlow 기반의 CNN(ResNet, YOLO 등) 모델 확장을 고려한 규격화된 Interface 구현

### 🎓 전공 지식 적용 포인트 (산업경영공학)
- **통계적 공정 관리(SPC):** 결함 데이터를 수집하여 공정 능력 분석(Process Capability Analysis) 및 관리도(Control Chart) 작성의 기초 데이터로 활용할 수 있도록 `line_id`, `timestamp` 등의 현장 데이터를 설계에 포함했습니다.
- **생산 운영 최적화:** 단순한 불량 판정을 넘어 `action_required` 속성을 통해 재작업(Rework) 최소화와 라인 균형(Line Balancing)을 고려한 현장 맞춤형 구조를 채택하였습니다.
"""

