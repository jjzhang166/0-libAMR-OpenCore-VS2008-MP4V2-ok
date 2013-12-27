========================================================================
    CONSOLE APPLICATION : amr-nb-dec-example Project Overview
========================================================================

AppWizard has created this amr-nb-dec-example application for you.

This file contains a summary of what you will find in each of the files that
make up your amr-nb-dec-example application.


amr-nb-dec-example.vcproj
    This is the main project file for VC++ projects generated using an Application Wizard.
    It contains information about the version of Visual C++ that generated the file, and
    information about the platforms, configurations, and project features selected with the
    Application Wizard.

amr-nb-dec-example.cpp
    This is the main application source file.

/////////////////////////////////////////////////////////////////////////////
Other standard files:

StdAfx.h, StdAfx.cpp
    These files are used to build a precompiled header (PCH) file
    named amr-nb-dec-example.pch and a precompiled types file named StdAfx.obj.

/////////////////////////////////////////////////////////////////////////////
Other notes:

AppWizard uses "TODO:" comments to indicate parts of the source code you
should add to or customize.

/////////////////////////////////////////////////////////////////////////////

���뷽ʽ
Mode 0 - AMR 4.75 - Encodes at 4.75kbit/s
Mode 1 - AMR 5.15 - Encodes at 5.15kbit/s
Mode 2 - AMR 5.9 - Encodes at 5.9kbit/s
Mode 3 - AMR 6.7 - Encodes at 6.7kbit/s
Mode 4 - AMR 7.4 - Encodes at 7.4kbit/s
Mode 5 - AMR 7.95 - Encodes at 7.95kbit/s
Mode 6 - AMR 10.2 - Encodes at 10.2kbit/s
Mode 7 - AMR 12.2 - Encodes at 12.2kbit/s
8~15λһЩ noise frames �ͱ���λ�Ķ��塣

��Ӧ֡�Ĵ�С
CMR Mode Frame size (bytes)
0 AMR 4.75 13
1 AMR 5.15 14
2 AMR 5.9 16
3 AMR 6.7 18
4 AMR 7.4 20
5 AMR 7.95 21
6 AMR 10.2 27
7 AMR 12.2 32

��������һ���򵥵ļ��㣬PCM16��AMR֮���ת��
Amr һ֡Ϊ20����

AMR 4.75Kbits/s:
ÿ�����������λ�� = 4750bits/s
ÿ20ms֡ռ�õ�λ�� = 4750bits/s / 50frames/s = 95bits
ÿ20ms֡ռ�õ��ֽ��� = 95bits / 8bits/byte = 11.875bytes - Բ����12�ֽڣ�����Ĳ�0
����һ���ֽڵ�֡ͷ�����ԣ�20msһ֡��AMR: 12-bytes + 1-byte = 13-bytes
�෴��ת�������ͳ���
13-bytes * 50frames/s * 8bits/byte = 5200bits/s
ע�⣬����������ֵ������Ӧ��������Բ����ԭ��
�༭����

�ļ���ʽ

Amr���ļ���ʽ��Ϊ�򵥣���ͼ1��ʾ��
�ļ��ʼʱ6���ֽڵ�header��
[#!AMR\n] ���ż�Ĳ���
(����ʮ�����Ʊ�ʾΪ 0x2321414d520a ).
��������������������֡��
ÿ��֡����һ��֡ͷ+��������
֡ͷ��ͼ2��ʾ��
P����Ϊ0
FTΪ����ģʽ�������Ѿ��о��˿��õ�ֵ��
QΪ֡����ָʾ�������Ϊ0����֡���𻵣���������Ҫ��RX_TYPE���ó�SPEECH_BAD����SID_BAD��
��ΪRX_TYPE��ο�RFC3267����ʵ�ýڽ��ܵ����ݶ�������RFC3267�����ҵ���
ͼ3 ���ͼ��Ϊ 5.9 kbit ������ļ���ʽ (with 118 speech bits)
����PΪ��0λ��
