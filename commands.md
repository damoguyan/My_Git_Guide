��װ����
=====================
(1)���� �����ֿ�ʱ�����˿���
$git config --global user.name "yourname"  //ע�����ʹ���ǳ��Ա�����˽
$git  config --global user.email "your_email@XX.com"
(2) �������������ӵ�и��ߵĿɶ���
$git config --global color.ui auto
(3)
�������þ�������~/.gitconfig�ļ��У�����Ҳ����ֱ�Ӵ������޸�����ļ�

�������
===========================
��������Working Directory----�����￴��Ŀ¼������test��
�汾�⣨Repository��-��������һ������Ŀ¼.git��������㹤����������Git�İ汾��
�汾������Ҫ��3��������
(1)�ݴ���stage�����߽�index��
(2)�Զ������ĵ�һ����֧'master'
(3)ָ��master��һ��ָ��'HEAD'
�ύ���̣� �������ļ�--->�ݴ���(add����ʵ��)---->����master(ͨ��commit����ʵ��)



======================
$mkdir test #������
$cd test 
$git init   #�汾��

�������� 
===================
$git  add file1 file2
$git  commit -m "message"
$git  status          #�ֿ⵱ǰ��״̬
$git  diff
$git  log
$git checkout -- file  #û��--���ͱ���ˡ��л�����һ����֧��������


�汾��ת
==============
�ص���ȥ
-----------
$git log
$git reset --hard commit_id   #(git�İ汾�Ų���1,2,3����hashֵ������������ְ汾��ǰ��λ����)
$git reset --hard  HEAD   #HEAD��ʾ��ǰ�汾 ��HEAD^  HEAD^^  HEAD~10���ֱ��ʾ��ǰ�汾��ǰһ����2�� 10���汾
ȥ���������δ��
-----------------
$git reflog   #�鿴������ʷ ��Ҫ��Ϊ�˿�commit_id
$git reset --hard commit_id 

ɾ���ļ�
=================
(1)�ȱ��ع�����ɾ��
$rm test.md
(2)ȷʵҪɾ���汾����ļ�
$git rm test.rm
(3)ɾ����
$git checkout -- test.md


Զ�ֿ̲�
==============
���͵�Զ��(github)
---------------------
(1)��һ��$ ssh-keygen -t rsa -C "youremail@example.com"  #�����ɵĹ�ԿKey��ӵ��Լ�github�˻���ssh������
(2)��github��վ�ϴ���repository��������My_Git_Guide
(3)������վ��ʾ���Լ������Ϸֱ�������������
$git remote add origin https://github.com/damoguyan/My_Git_Guide.git #��һ�����еı��زֿ���֮����
$git push -u origin master  #�ѵ�ǰ��֧master���͵�Զ�� ��һ�μ�-u
(4)���������иĶ������͵�Զ��
$git push origin master

��Զ��clone
--------------------
$git clone git@github.com:damoguyan/bitcoinbook.git #Git֧�ֶ���Э�飬����https����ͨ��ssh֧�ֵ�ԭ��gitЭ���ٶ����


