# last-lesson


vm

https://classroom.udacity.com/nanodegrees/nd013/parts/6047fe34-d93c-4f50-8336-b70ef10cb4b2/modules/e1a23b06-329a-4684-a717-ad476f0d8dff/lessons/7e3627d7-14f7-4a33-9dbf-75c98a6e411b/concepts/8c742938-8436-4d3d-9939-31e40284e7a6


pip update

wget https://bootstrap.pypa.io/get-pip.py

でバージョンアップされたpipを直接ダウンロードして

sudo python3 get-pip.py

で普通にインストールしたらでけた。


udacity project (github site repository)

https://github.com/udacity/CarND-Capstone



### VirtualBox 共有設定（フォルダ登録
①VirtualVMに仮想光学ドライブを追加　内容は空ディスクでOK
②VirtualVMメニューの「Device」→「Insert Guest Additions CD images ...」．を選択起動（成り行きOK）
③Guest Additions CDイメージをマウント
# mount /dev/cdrom /適当なフォルダ
④仮想CDの中に入っている./VBoxLinuxAdditions.runを実行する
# ./VBoxLinuxAdditions.run
終わったら仮想マシンは、一旦シャットダウンする。
# shutdown -h now


### VirtualBox 共有設定（パーミッション解放）
以下　トライして再起動　
Add yourself to the vboxsf group within the guest VM.
・Solution 1
Edit the file /etc/group. Look for the line vboxsf:x:999 and add at the end :yourusername

・Solution 2
Run sudo adduser $USER vboxsf

