# はじめに
NebulaFlowは、継続的インテグレーション・継続的デリバリーを駆使したコード品質管理ツールである。
絶え間ないデプロイの中でコードの品質を保っていくために、コード品質管理ツールを使って、継続監視・またその指摘内容を統計化することで完全なコード管理を実現する。

NebulaFlowを取り入れた企業はエンジニアスキルの向上だけでなく、IT戦略の大きなアドバンテージを実現する。

NebulaFlowは、コーディングをアナーキーなブラックホールではなく、星雲の天の川のような煌びやかさを兼ね備えた、保守・運用を可能とする。

# 参考文献

[SonarQube Docs](https://docs.sonarsource.com/sonarqube/latest/)

# Common Setting

## ネットワーク作成

```
[実行コマンド]
docker network create --subnet=172.10.10.0/24 --gateway=172.10.10.1 nebula_net

[確認コマンド]
docker network list
```

## Volume作成

```
[実行コマンド]
docker volume create nebula_vol
docker volume create gitlab_config
docker volume create gitlab_logs
docker volume create gitlab_data

[確認コマンド]
docker volume list

[結果]
```