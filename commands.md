��װ
=====================
$git config --global user.name "yourname"
$git  config --global user.email "your_email@XX.com"

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
