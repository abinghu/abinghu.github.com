### 1. ����mingw����shell���������ʾ��

#### ������ʾ
�������ļ�/etc/profile���������룬

    export LANG=en

    alias l='/bin/ls --show-control-chars --color=auto'
    alias la='/bin/ls -aF --show-control-chars --color=auto'
    alias ll='/bin/ls -alF --show-control-chars --color=auto'
    alias ls='/bin/ls --show-control-chars --color=auto'

#### ��������
��/etc/inputrc.default���û�Ŀ¼�µ�.inputrc�ļ��е�������޸�Ϊ�������ݣ�

    set meta-flag on
    set input-meta on
    set output-meta on
    set convert-meta off

### 2. ��װwget���
����mingw�Դ���װ��wget�汾���ϣ�������Ҫ����wget���
    
    mingw-get update // ����mingw�İ�װ����Ϣ
    mingw-get show | grep 'wget' // ��ʾwget��װ���������Ϣ
    mingw-get install msys-wget  // ��װ���°��wget��װ��

### 3. ʹ��wget����avlog���񻰵����������¼
avlog.avplayer.org��վʹ��httpsЭ�飬��wget���������ѡ��

    wget -r -nd -np --no-check-certificate 'https://avlog.avplayer.org/��/'
���к�ᷢ��wget��֧�����ĵĴ��룬��wget�������Ϣ�п��Է��֣�wget��urlʶ��Ϊ

    https://avlog.avplayer.org/%C9%F1%BB%BO

����ܿ�������Ϊmingw console��GBK�����Ե�ʣ���wget����unicode�ķ�ʽȥ���������񻰡����֣����յ���wget connect��ʱ��û�з��ֶ�Ӧ���ļ���ûӡ֤������������wget��֧������url�����⣬�����������������һ�����޸�Դ���루google֮��ֻ��Ҫ���޸ļ��д���Ϳ����ˣ�����һ�ַ����Ǵ��������url������url��gvim�У�Ȼ���ٽ���ת�����url��Ϊwget��url�����Ϳ����ˣ�������ʾ��
    
    https://avlog.avplayer.org/%E7%A5%9E%E8%AF%9D
