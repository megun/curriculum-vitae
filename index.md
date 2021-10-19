# 職務経歴書

## 基本情報

| | |
|---|---|
|名前|megun|
|住所|都内在住|
|学歴|専門学校　情報処理科　卒業|
|資格|2001/11 日商簿記2級<br>2011/12 旧情報セキュリティスペシャリスト試験<br>2013/01 OracleBronze<br>2015/09 LPIC-Lv.3(core)<br>2017/05 RubySliverVer2.1|
|趣味|ギター<br>近所の猫スポット探し|

## 概要
- 専門学校卒業後、SI企業に就職し正社員として業務に携わる
  - 金融系のデータセンターで監視、運用設計など
  - ホスティングサービスの構築、運用、障害対応など
- 下記のような思いからフリーランスになる
  - 業務委託が多くフリーランスで働くのと変わらないと感じた。
  - 色々な所で経験を積んでスキルアップしたかった
  - そのまま正社員で続けた場合、技術職で続けてくのが難しそうに思った
    - マネージメント系は自分には向いてないと思った
- ずっとインフラ系エンジニアやってる

## できること
- インフラコード管理
  - 構成管理ツール系は一通り実務経験ある。
  - Terraform
    - 勉強および備忘録として[サンプル](https://github.com/megun/terraform-samples)書くことを始めた
  - CloudFormation
    - メインでがっつりやった経験はないけど、書いたことはある。
  - Ansible
    - ブランクあるけど、普通に書けるはず。 [サンプル](https://github.com/megun/ansible-samples)
- AWS関連の構築、運用
  - 一通りのサービスは構築、運用した経験ある
- コンテナ系
  - Kubernetes(EKS)構築、運用できる
    - 各種ツール(eksctl,kubectlなど)使って構築、運用（トラブル調査とか）できる
    - manifest書ける
    - istio何とかいける
  - ECS構築、運用経験ある
- 監視系
  - Datadog
    - モニタやダッシュボード作ったり一通りの経験はある
- CI/CD系
  - GithubActions
    - Dockerイメージのビルド、イメージプッシュ、デプロイなどで利用経験ある
  - CircleCI
    - Dockerイメージのビルド、イメージプッシュ、デプロイなどで利用経験ある
  - Spinnaker
    - 構築してeksへのデプロイ、バージョンアップなど一通りの経験はある
  - ArgoCD
    - 設計、構築、eksへのデプロイまで一通りの経験はある
- その他
  - インフラ系全般で幅広く経験してきてる
    - オンプレサーバのラッキングからOS、ミドルウェア設定とか
    - 仮想環境の管理
    - 各ミドルウェアの管理
    - ネットワーク機器（スイッチ、ルータ）の管理

## できないこと
- ちゃんとしたプログラム書くこと
  - 運用系スクリプトで複雑なものでなければ読めるし書ける
- 英語
  - google翻訳とかないと無理
  - 勉強しようとは思ってる

## 興味、今後やりたいこと
- AWSなどのクラウド関連については、今後も継続的にやっていきたい。
- kubernetesなどのコンテナ関連についてもっと経験を積みたい。

<div style="page-break-before:always"></div>

## 職務経歴（フリーランス）

### AIサービスのインフラ環境構築、保守 (2021/10 - 2021/10)
<details open>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - AI×SaaSプロダクトのインフラ業務
  - インフラチームは9人
  - EKS上でサービス稼働
- 業務内容
  - 新規環境構築
    - 脆弱性診断用の環境構築
  - 物理マシンへの既存アプリケーション移行のフォロー
    - メイン作業は別の人(アプリケーションチームの人)
    - インフラ関連(k8s/istioとか)をフォローする感じ
- 利用ツール、サービスなど
  - Terraform,eksctl,aws-cli
  - EKS,EC2,RDS(AuroraAurora),S3,SQS
  - kubectl,kustomize,helm,istio
  - ArgoCD,ArgoWorkflow,ArgoEvent

</div>
</details>


### 育休期間 (2021/04- 2021/09)

育休

### ブロックチェーン関連サービスのインフラ環境構築、保守 (2020/04 - 2021/03)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - 決済プラットフォームサービスのインフラ構築保守全般を担当
  - インフラ専任は一人
  - EKS上で各種マイクロサービス起動、Istioでサービスメッシュ構成
  - 環境数は4～7面（時期によって増減する）くらい。
- 業務内容
  - AWS上に構築されたインフラ環境の構築、保守全般
    - 不要リソースの調査、削除の提案
  - Kubernetes(EKS)環境の構築、保守全般
    - 各種ツールの利用提案(ClusterAutoscaler,metrics-server,kube-state-metricsなど)
    - Secret管理方法の改善提案（ExternalSecrets+ParameterStore）
  - CI/CDの改善活動
    - SpinnakerからArgoCDへの移行提案、構成設計、実装
    - manifestのvalidationをGithubActions/CircleCIで実装(kubeval,kube-score)
  - 監視環境の構築、改善活動
    - 監視項目検討、実装、修正
    - Dashbordの整備
  - 技術検証
    - Spinnakerのバージョンアップ検証
    - ArgoCDの機能検証、構成検討
    - EKSバージョンアップ方法の検証
    - istio1.4から1.7系へのバージョンアップ方法の検証
    - AppMeshの機能検証
    - EFSの機能検証
    - データ分析用途としてMetabase提案、実装
  - 運用スクリプト作成、保守
    - Bashスクリプト
    - datadogへメトリクス通知するGoスクリプト作成
- 利用ツール、サービスなど
  - Terraform,eksctl,aws-cli
  - EKS,EC2,RDS(AuroraPostgreSQL),Elasticache(Redis),Lambda,SES,CloudFront,S3,SystemManager,KMS,EFS
  - kubectl,kustomize,kubeval,kube-score,external-dns,kubernetes-external-secrets,metrics-server,istio
  - Spinnaker,ArgoCD,GithubActions,CircleCI
  - Datadog,DatadgoLogs
  - Bash,Go
  - Metabase
</div>
</details>

### EC向けAPIプラットフォームサービス保守運用 (2019/09 - 2020/03)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - ECサイトのバックエンドとして各種APIを提供するサービス
  - インフラチームとしては6人ほど
  - 各顧客ごとにAWSアカウントあり、ECS上にマイクロサービス展開
  - 規模は顧客数\*環境(prod/devなど)で20ぐらいのAWSアカウント面倒見る
- 業務内容
  - 各顧客ごとのAWS環境の構築、保守全般
    - Bashスクリプト、CloudFormationなどでAWSリソース作成
    - アプリケーションのデプロイ
  - 運用スクリプト作成、保守
    - bashスクリプト、Pythonスクリプト
- 利用ツール、サービスなど
  - CloudFormation,Terraform,aws-cli,Ansible
  - ECS,Fargate,EC2,RDS(AuroraMySQL),Elasticache(Redis),DynamoDB,Lambda,SES,S3,SystemManager,Kinesis,SQS
  - Atlantis
  - Datadog,Sentry,CloudWatchLogs,td-agent,Elasticsearch
  - Bash,Python
</div>
</details>

### クラウド導入支援サービス (2018/07 - 2019/07)
<details>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - APNプレミアコンサルティングパートナーでのAWS環境の構築・運用業務
  - 所属したチームは4名ほどの規模
  - 主にゲーム系システムで環境数(prod/devなど)は顧客よるが3～5くらいはある。
  - 3～4つくらいの案件をメインで担当
- 業務内容
  - 各顧客ごとのAWS環境の構築、保守全般
    - terraform,ansible,chefなどの各種構成管理ツールでの基盤構築
    - 顧客からの問い合わせ対応
    - AmazonLinux2への入れ替え対応
    - ECS用EC2インスタンスのディスク枯渇対応(原因特定、ディスクサイズ変更)
  - 技術検証
    - Linuxアカウント管理としてstnsの検証、導入
    - ECSでRedash/Metabaseの検証、導入
    - EKSの検証、Spinnakerの検証
- 利用ツール、サービスなど
  - Terraform,Packer,aws-cli,Ansible,Chef(Knife-zero)
  - ECS,Fargate,EC2,RDS(AuroraMySQL,PostgreSQL),Elasticache(Memcache,Redis),Lambda,SES,S3,SystemManager
  - CodeDeploy,CodeBuild,Rundeck,Jenkins
  - Datadog,Mackerel,td-agent,Elasticsearch
  - Bash,Python,Ruby
  - nginx,apache,ldap
</div>
</details>

### 国内クラウドサービスの新規開発 (2017/06 - 2018/06)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - 新規クラウドサービスの開発
  - 所属したチームは6～8名でインフラ専任は一人
  - CloudStackで基盤構築されてるがそこは別チーム担当でOSレイヤー以上を担当
- 業務内容
  - インフラ環境構築
    - OS、ミドルウェア、監視周りの設定
    - ログ収集機能がなかったのでEFK提案、構成設計、実装
  - デプロイ環境構築
    - Capistranoでアプリケーションデプロイ基盤を構築
  - 軽微なアプリケーション修正、アプリケーション機能開発
    - CloudStackでVM作成、Userdataでルーティング追加する
    - Sensu監視設定
- 利用ツール、サービスなど
  - Ansible
  - CloudStack
  - Capistrano
  - Zabbix,Sensu,td-agent,Elasticsearch,Kibana
  - Bash,Ruby
  - nginx,RabbitMQ,Redis,PerconaXtraDB,MySQL,DRBD,HAProxy
</div>
</details>

### 不動産系システムのインフラ構築、運用、保守 (2016/10 - 2017/04)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - ホスティングサービスで稼働してる既存システムをAWSへ移行する
  - インフラ担当は二名
- 業務内容
  - AWSクラウドへのインフラ環境構築、運用、保守
    - AWS各リソースの設計、構築
    - OS、ミドルウェア、監視周りの設定
  - 既存システムの調査
- 利用ツール、サービスなど
  - EC2,CloudFront,RDS,S3,Elasticache
  - Mackerel
  - Bash,PHP
  - Apache,Wordpress
</div>
</details>

### 広告配信システムインフラ構築／運用・保守  (2015/08 - 2016/09)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - オンプレ、クラウドで稼働してるサービスのインフラ構築／運用・保守
  - インフラ担当は二名
- 業務内容
  - OS/ミドルウェア構築
    - KickstartでOSインストール(4-50台くらい)
    - Ansibleで各種ミドルウェア設定
    - Redis/MongoDBのローリングアップデート実施
  - 障害対応／調査
    - MySQL容量枯渇対応（パーティショニング設定、過去データバックアップ、定期的な不要データの削除自動化など実施）
  - アプリケーションデプロイ
    - Ansibleでアプリケーションデプロイ
- 利用ツール、サービスなど
  - Ansible
  - CentOS6-7,Gentoo
  - MariaDB,MongoDB
  - Zabbix
  - Nginx,Redis,Yrmcds,Hadoop,keepalived
</div>
</details>

### 自動車関連の情報提供会社のSEサポート業務  (2015/04 - 2015/07)
<details close>
<summary>詳細</summary>
<div>

- プロジェクト概要
  - XenServerに構築された各種システムの保守
- 業務内容
  - FW/LB/DNS設定変更
    - 顧客帯合わせに従い各種NW機器の設定変更
  - 障害調査／対応
    - アラートを受けて障害対応（できることはサービス再起動とかそのくらいだった）
- 利用ツール、サービスなど
   - XenServer
   - CentOS5-6
   - PostgreSQL,MySQL
   - Apache,Keepalived,BIND
   - Juniper(FW),BIG-IP(LB)
</div>
</details>

### 職業紹介会社のインフラ環境の構築  (2013/12 - 2015/03)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - 各プロジェクトのインフラ構築
  - オンプレ、VMware
- 業務内容
  - 仮想サーバの設計構築
  - NW設備の設定変更
  - 保守担当者への引継ぎ
- 利用ツール、サービスなど
  - VMware Vsphere
  - CentOS6,WindowsServer2008,WindowsServer2012
  - PostgreSQL
  - Zabbix
  - DRBD,Heartbeat,Pacemaker
  - Apache,Tomcat
  - Cisco2960,CiscoASA,BIG-IP
</div>
</details>

## 職務経歴（正社員）

### 金融機関の社内インフラ移行案件  (2013/02 - 2013/11)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - 社内システム（メール、Web閲覧など）の刷新
  - 実際に手を動かすのは別会社が担当、設計レビューなどを担当
- 業務内容
  - 設計レビュー
  - ユーザマニュアル作成
  - テスト項目策定
  - ベンダーへの指示管理業務
- 利用ツール、サービスなど
  - VMware Vsphere
  - RHEL6
  - Apache,Squid,BIND,Sendmail
  - I-Filter
  - InterScanWebSecurityVirtualAppliance,InterScanMessagingSecurityVirtualAppliance
  - SymantecMessagingGatewayVirtualEdition
  - CheckPoint(FW),Cisco(SW),A10(LB),
</div>
</details>

### 通信キャリアDCにて運用・保守業務  (2010/02 - 2012/10)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - ホスティングサービスの運用・保守業務
- 業務内容
  - ホスティングサーバの構築
  - エンドユーザからの問い合わせ対応
  - 障害対応、パッチ適用などの保守メンテ作業
- 利用ツール、サービスなど
  - VMware Vsphere
  - RHEL5,6
  - MySQL,PostgreSQL
  - Apache,Squid,BIND,Sendmail,Webmin
  - I-Filter
  - InterScanWebSecurity,InterScanMessagingSecurity,InterScanWebManager
  - BackuExec
  - McAfee ePolicy Orchestrator,VirusScanEnterprise
  - NetScreen(FW),FortiGate(FW),Cisco(SW),Array(LB),ServerIron(LB)
</div>
</details>

### 社内向けの研修講師 (2008/02 - 2010/02)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - 社内向けの研修講師
- 業務内容
  - インフラ技術者育成の研修講師
  - 研修内容策定、研修用機器選定
  - 案件のヘルプ
- 利用ツール、サービスなど
  - HP-UX11,WindowsServer2003
  - Oracle11g
  - JP1製品
  - DataProtector,Arcserve
  - ServiceGuard,MSCS(MicrosoftClusterService)
  - ShellScript,VBScript
</div>
</details>

### 金融系データセンターでの運用設計、構築業務  (2003/04 - 2008/02)
<details close>
<summary>詳細</summary>

<div>

- プロジェクト概要
  - 金融系データセンターでの運用設計、構築業務
- 業務内容
  - JP1製品を使用したジョブ、監視設計/構築
  - 運用部への引継ぎ
  - スケジュール管理、顧客対応、チーム内への技術支援
- 利用ツール、サービスなど
  - Windows2000Server,WindowsServer2003,HP-UX,AIX,RHEL
  - JP1製品,Tivoli製品
  - Arcserve,BackuExec
  - ShellScript,VBScript,ExcelVBA,Perl
</div>
</details>
