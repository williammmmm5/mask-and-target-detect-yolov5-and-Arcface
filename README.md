Face Mask Compliance Monitor

This project integrates a face detection model trained with YOLOv5 and ArcFace for target recognition to monitor and enforce face mask compliance in public spaces. If an individual is detected without a mask more times than the set threshold, the system will notify concerned personnel through Slack. The service is built using FastAPI for easy web deployment.
-
Features
-

    Face Detection: Real-time face detection using a model trained with YOLOv5.
    Identity Verification: Accurate target recognition through ArcFace, linked with a face database.
    Mask Compliance Check: Sequential detection of correct mask usage with a specially trained model.
    Non-compliance Notification: Sends alerts through Slack when an individual's non-compliance with mask-wearing reaches the limit.
    Web Service: Built with FastAPI for easy web deployment and integration.

Installation
-

Ensure you have Python 3.8 or higher installed and then install all necessary dependencies.

bash
-

git clone https://github.com/yourusername/face-mask-compliance-monitor.git
cd face-mask-compliance-monitor
pip install -r requirements.txt

Usage
-

    Start the FastAPI server:

    bash

    uvicorn main:app --reload

    Access http://127.0.0.1:8000/docs to view the API documentation and test endpoints.
    Connect your camera feed to the service to start real-time monitoring and analysis.

Contributing

Contributions to the project are welcome. If you have suggestions or improvements, please submit an issue or pull request.
License

This project is licensed under the MIT License.
--------------------------------------------------------------------
マスク着用遵守モニター

このプロジェクトは、公共の場でのマスク着用を監視し、強化するために、YOLOv5で訓練された顔検出モデルとArcFaceを使用したターゲット認識を統合しています。特定の個人が設定された閾値以上にマスクを着用していないと検出された場合、システムはSlackを通じて関係者に通知します。このサービスは、Webデプロイメントを容易にするためにFastAPIを使用して構築されています。
特徴

    顔検出: YOLOv5で訓練されたモデルを使用したリアルタイム顔検出。
    身元確認: ArcFaceによる正確なターゲット認識、顔データベースとのリンク。
    マスク着用チェック: 専用に訓練されたモデルで正しいマスクの着用を順次検出。
    違反通知: 個人のマスク非着用が限度に達すると、Slackを通じて警告を送信します。
    Webサービス: FastAPIで構築されたWebサービスで、簡単にデプロイメントと統合が可能です。

インストール

Python 3.8以上がインストールされていることを確認し、必要な依存関係をすべてインストールしてください。

bash

git clone https://github.com/yourusername/face-mask-compliance-monitor.git
cd face-mask-compliance-monitor
pip install -r requirements.txt

使用方法

    FastAPIサーバーを起動します：

    bash

    uvicorn main:app --reload

    http://127.0.0.1:8000/docsにアクセスして、APIドキュメントを表示し、エンドポイントをテストします。
    カメラフィードをサービスに接続して、リアルタイムの監視と分析を開始します。

貢献

プロジェクトへの貢献を歓迎します。提案や改善がある場合は、IssueやPull Requestを送ってください。
ライセンス

このプロジェクトは MIT License のもとでライセンスされています。
