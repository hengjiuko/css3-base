                       ѧϰCSS3�ıʼ�
1.�߿�Բ��Ч����border-radius:5px 4px 3px 2p;/*�ĸ��뾶�ֱ������Ͻǡ����Ͻǡ����½Ǻ����½ǣ�˳ʱ��*/
2.�߿���Ӱ��box-shadow:X��ƫ�� Y��ƫ�� [��Ӱģ���뾶] [��Ӱ��չ�뾶] [��Ӱ��ɫ] [ͶӰ��ʽ]��
   ͶӰ��ʽ:insetΪ�ڲ���Ӱ��ʽ��ʡ��Ϊ�ⲿ��Ӱ��ʽ��inset����д�ڲ����ĵ�һ�������һ����
3.border-image(Ϊ�߿�Ӧ��ͼƬ)��url(borderimg.png) 70 repeat 
   Round���������ΪԲ��������
   Stretch���������Ϊ����
4.��ɫ֮ RGBA
   �﷨��color:rgba(100,120,60,0.5)
 Aָ��RGB�����Ͽ���alpha͸���ȵĲ���
5.css3������ɫ
  css3 Gradient��Ϊ���Խ��䣨linear���;��򽥱�(radial)
    linear-gradient(to bottom,#fff,#999)
                 /*���䷽��*/ /*��ʾ��ɫ����ʼ��ͽ����㣬�������������ɫֵ*/
6.css3����������text-overflow��word-wrap
  text-overflow:clip    |    ellipsis
          /*��ʾ����*/    /*��ʾ��ʾʡ�Ա��*/
 ��Ҫʵ�����ʱ����ʡ�Ժŵ�Ч�������붨��ǿ���ı���һ������ʾ��white-space:nowrap�����������Ϊ���أ�overflow:hidden����ֻ����������ʵ������ı���ʾʡ�Ժŵ�Ч�����������£�
    text-overflow:ellipsis; 
    overflow:hidden; 
    white-space:nowrap;
       word-wrapҲ�������������ı���Ϊ����ǰ�г���ָ�������ı߽�ʱ�Ƿ�Ͽ�ת��
  �﷨��word-wrap:normal     |    break-word
   /*��ʾ���������ı�����*/  /*��ʾ���ݽ��ڱ߽��ڻ���*/
7.Ƕ������@font-face
    �﷨:  @font-face {
         font-family : ��������;
         src : �����ļ��ڷ������ϵ���Ի����·��;
     }
    ��������֮�󣬾Ϳ�����ʹ����ͨ����һ���ڣ�font-*��������������ʽ��

   ���磺p {
          font-size :12px;
          font-family : "My Font";
          /*���������@font-face��font-familyͬ����ֵ*/
       }
8.�ı���Ӱtext-shadow
   �﷨��text-shadow: X-Offset Y-Offset blur color;
   X-Offset����ʾ��Ӱ��ˮƽƫ�ƾ��룬��ֵΪ��ֵʱ��Ӱ����ƫ�ƣ���֮����ƫ�ƣ�      

   Y-Offset����ָ��Ӱ�Ĵ�ֱƫ�ƾ��룬�����ֵ����ֵʱ����Ӱ����ƫ�ƣ���֮����ƫ�ƣ�

   Blur����ָ��Ӱ��ģ���̶ȣ���ֵ�����Ǹ�ֵ�����ֵԽ����ӰԽģ������֮��ӰԽ�������������Ҫ��Ӱģ�����Խ�Blurֵ����Ϊ0��
   Color����ָ��Ӱ����ɫ�������ʹ��rgbaɫ��
9.�뱳����ص���ʽ
  1>background-origin:border-box | padding-box | content-box;
  ���ñ���ͼƬ��ԭʼ��ʼλ�ã������ֱ��ʾ����ͼƬ�Ǵӱ߿򣬻����ڱ߾ࣨĬ��ֵ������������������ʼ��ʾ��
  2>background-clip:border-box | padding-box | content-box | no-clip
  ����������ͼƬ���ʵ��Ĳü�����Ӧʵ����Ҫ�������ֱ��ʾ�ӱ߿򡢻�����䣬����������������ü�������no-clip��ʾ�����У��Ͳ���border-box��ʾͬ����Ч����backgroud-clipĬ��ֵΪborder-box��
  3>background-size: auto | <����ֵ> | <�ٷֱ�> | cover | contain
          �������ñ���ͼƬ�Ĵ�С
   cover��������ͼƬ�ȱ���������������������
   contain�����ɣ���������ͼƬ�ȱ�������ĳһ�߽���������ԵΪֹ��
  4>multiple backgrounds
  �﷨��д��background �� [background-color] | [background-image] | [background-position][/background-size] | [background-repeat] | [background-attachment] | [background-clip] | [background-origin],...


















