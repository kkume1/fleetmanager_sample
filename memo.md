EC2につける権限
・SessionManagerアクセス許可　　：AmazonSSMManagedInstanceCore
・FleetManagerアクセス許可Fleet ：Managerのアクセス許可を持つ IAM ポリシー

権限はAmazonSSMManagedInstanceCoreのみでファイルシステムとユーザーは表示OK
プロセスはkmsの"Allow use of the key"にロールのarnを入れる

kmsのkey作成時に使用者にロールを入れると
"Allow use of the key"にもロールがプリンシパルに入る。