��װ
=====================
$git config --global user.name "yourname"
$git  config --global user.email "your_email@XX.com"


�����ֿ�(repository)
======================
$mkdir test
$cd test 
$git init

�������� 
===================
$git  add file1 file2
$git  commit -m "message"
$git  status          #�ֿ⵱ǰ��״̬
$git  diff
$git  log


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
