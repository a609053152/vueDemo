������Ҫ����ɲ��֣���ͼ���ű�
el��idѡ����
data���������ݣ���ֵ
�������ڣ�ҳ���ʼ��ǰ�󣬹���ǰ��������ĺ���������Ӧ��API���ã���������
ģ���﷨ -��ֵ��֧��JS���ʽ���������㣩  ��Ԫ���ʽ���ȽϽ��Ϊ��ִ�У�������룬�Ƚ�ʧ��ִ�У�������룩��Html��ǩƴ�ӣ�������.split()��
ģ���﷨ -ָ�v-if��������ʾ�� v-bind:href="url" ��ת  @click����¼�
Class �� Style �󶨣���̬��ʾ��ʽ
������Ⱦ��v-if ��ֵ��ʲô����ʾʲô
�б���Ⱦ��v-for ָ����Ҫʹ�� item in items ��ʽ�������﷨������ items ��Դ�������飬�� item ���Ǳ�����������Ԫ�صı�����
�¼���: v-on ������ v-on ָ����� DOM �¼������ڴ���ʱ����һЩ JavaScript ����,�ṩ�˺ܶ��¼����η�������  v-on���԰�����HTML�¼���dblclike��˫���¼���

������󶨣������� v-model ָ���ڱ� <input>��<textarea> �� <select> Ԫ���ϴ���˫�����ݰ󶨡�������ݿؼ������Զ�ѡȡ��ȷ�ķ���������Ԫ�ء�������Щ���棬�� v-model �����ϲ������﷨�ǡ�����������û��������¼��Ը������ݣ�����һЩ���˳�������һЩ���⴦��
v-model ��������б�Ԫ�ص� value��checked��selected attribute �ĳ�ʼֵ�����ǽ� Vue ʵ����������Ϊ������Դ����Ӧ��ͨ�� JavaScript ������� data ѡ����������ʼֵ��v-model ���ڲ�Ϊ��ͬ������Ԫ��ʹ�ò�ͬ�����Բ��׳���ͬ���¼���

text �� textarea Ԫ��ʹ�� value ���Ժ� input �¼���
checkbox �� radio ʹ�� checked ���Ժ� change �¼���
select �ֶν� value ��Ϊ prop ���� change ��Ϊ�¼���


���������Vue.component���ע��  ����ǿɸ��õ� Vue ʵ�����Ҵ���һ�����֣�������������� <button-counter>�����ǿ�����һ��ͨ�� new Vue ������ Vue ��ʵ���У�

���ע�� ��һ���������ȫ��ע��Ҳ���Ծֲ�ע��  components 
new Vue({
  el: '#app',
  components: {
    'component-a': ComponentA,
    'component-b': ComponentB
  }
})

���ļ������ȫ�ֶ��� (Global definitions) ǿ��Ҫ��ÿ�� component �е����������ظ�
�ַ���ģ�� (String templates) ȱ���﷨�������� HTML �ж��е�ʱ����Ҫ�õ���ª�� \
��֧�� CSS (No CSS support) ��ζ�ŵ� HTML �� JavaScript �����ʱ��CSS ���Ա���©
û�й������� (No build step) ����ֻ��ʹ�� HTML �� ES5 JavaScript, ������ʹ��Ԥ���������� Pug (formerly Jade) �� Babel
