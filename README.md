# easyUtil_poped
Modal Dialogue Box by  JavaScript
<h3>���</h3>
		<h4>&emsp;&emsp;easyUtil.poped�Ǽ򵥵�ģ̬�������ڣ�ӵ����ʾ�򣬾���򣬶Ի����Լ��������ڹ��ܣ���������ɫ��ʽ����ѡ��Ҳ�����Զ�����ʽ���޸�css�ļ���Ӧ�༴�ɡ�</h4>
		<h4>&emsp;&emsp;easyUtil.poped֧��ģ�黯����</h4>
		<h3>API:</h3>
		<h3>���</h3>
		<ul>
			<li>1.��ͨ����ȫ����������ΪeasyPoped��ģ�黯���Զ�������</li>
			<li>2.��֤easyUtilPoped_v1.0�ļ���Ŀ¼�ṹ��������ŵ���ĿĿ¼�£������ļ�����</li>
		</ul>
		<h3>���巽��������������ͨ��������Ϊ����</h3>
		<ul>
			<li>1. ��ʾ��
				<p>easyPoped.msg(text, time, offset): </p>
				<p>&emsp;&emsp;text�� String��Number���ͣ���ʾ���ݣ� </p>
				<p>&emsp;&emsp;time��ѡ���� ,Ĭ��1000ms, Number���ͣ��Զ��ر�ʱ�� ms ��Ϊ0���ֶ��رգ��粻���ô��Ҳ��ֱ��дoffsetƫ����</p>
				<p>&emsp;&emsp;offset��ѡ��� Array���ͣ�������ƫ����top,left����ֵ����ֻдһ��ֵ��������topƫ�ƣ�֧�ֶ��ֵ�λ�Ͱٷֱȣ������д��λ��Ĭ��px��</p>
				<p>&emsp;&emsp;��������ֵΪ��ǰ��ʾ���id,����ֶ��رգ�����Խ�id����closeMsg�������ر���ʾ��</p>
			</li>
			<li>2. �������ڣ�
				<p>easyPoped.open(option): </p>
				<p>&emsp;&emsp;option = {<br/>
					&emsp;&emsp;&emsp;&emsp;title�� �������ڵı��⣻<br/>
					&emsp;&emsp;&emsp;&emsp;url�� ����ҳ���url��ַ��<br/>
					&emsp;&emsp;&emsp;&emsp;space�� ѡ���Ĭ��[50%��50%],�������ͣ������㴰�ڿ�ߣ���ֻдһ��ֵ��������width��֧�ֶ��ֵ�λ�Ͱٷֱȣ������д��λ��Ĭ��px��<br/>
					&emsp;&emsp;&emsp;&emsp;style�� ѡ���������ʽ��1.��ɫ��Ĭ�ϣ���2.��ɫ��<br/>
					&emsp;&emsp;&emsp;&emsp;closeBtn�� ѡ������Ͻǹر���ʽ��1.��ɫ��Ĭ�ϣ���2.��ɫ���粻��Ҫ������0��<br/>
					&emsp;&emsp;&emsp;&emsp;outClose�� ѡ���������ֲ��Ƿ���Թرգ�Ĭ��true���ɹرգ�<br/>
					&emsp;&emsp;&emsp;&emsp;closeFn�� ѡ����رմ��ں�Ļص�������<br/>
				&emsp;&emsp;}</p>
			</li>
			<li>3. �����
				<p>easyPoped.alert(option): </p>
				<p>&emsp;&emsp;option = {<br/>
					&emsp;&emsp;&emsp;&emsp;title�� ���洰�ڵı��⣻<br/>
					&emsp;&emsp;&emsp;&emsp;content���������ݣ�<br/>
					&emsp;&emsp;&emsp;&emsp;icon�� ѡ�����ʾͼ��,0�ޣ�1���棬2�ɹ���Ĭ�ϣ���3ʧ�ܣ�4ѯ�ʣ�<br/>
					&emsp;&emsp;&emsp;&emsp;style�� ѡ���������ʽ��1.��ɫ��Ĭ�ϣ���2.��ɫ��<br/>
					&emsp;&emsp;&emsp;&emsp;closeBtn�� ѡ������Ͻǹر���ʽ��1.��ɫ��Ĭ�ϣ���2.��ɫ���粻��Ҫ������0��<br/>
					&emsp;&emsp;&emsp;&emsp;outClose�� ѡ���������ֲ��Ƿ���Թرգ�Ĭ��false�����ɹرգ�<br/>
					&emsp;&emsp;&emsp;&emsp;btn: ѡ����������ͣ���ť�����ƣ�Ĭ��"ȷ��"��<br/>
					&emsp;&emsp;&emsp;&emsp;btnsRML: ��ť��λ�ã�"r".���ң�Ĭ�ϣ�,"m".����,"l".����<br/>
					&emsp;&emsp;&emsp;&emsp;btnFn�� ѡ������ȷ�ϰ�ť��Ļص�������<br/>
				&emsp;&emsp;}</p>
			</li>
			<li>4. ȷ�Ͽ�
				<p>easyPoped.confirm(option): </p>
				<p>&emsp;&emsp;option = {<br/>
					&emsp;&emsp;&emsp;&emsp;title�� ȷ�ϴ��ڵı��⣻<br/>
					&emsp;&emsp;&emsp;&emsp;content��ȷ�����ݣ�<br/>
					&emsp;&emsp;&emsp;&emsp;icon�� ѡ�����ʾͼ��,0�ޣ�1���棬2�ɹ���3ʧ�ܣ�4ѯ�ʣ�Ĭ�ϣ���<br/>
					&emsp;&emsp;&emsp;&emsp;style�� ѡ���������ʽ��1.��ɫ��Ĭ�ϣ���2.��ɫ��<br/>
					&emsp;&emsp;&emsp;&emsp;closeBtn�� ѡ������Ͻǹر���ʽ��1.��ɫ��Ĭ�ϣ���2.��ɫ���粻��Ҫ������0��<br/>
					&emsp;&emsp;&emsp;&emsp;outClose�� ѡ���������ֲ��Ƿ���Թرգ�Ĭ��false�����ɹرգ�<br/>
					&emsp;&emsp;&emsp;&emsp;btn1: ѡ�����ť1�����ƣ�Ĭ��"ȷ��"��<br/>
					&emsp;&emsp;&emsp;&emsp;btn2: ѡ�����ť2�����ƣ�Ĭ��"ȡ��"��<br/>
					&emsp;&emsp;&emsp;&emsp;btnsRML: ��ť��λ�ã�"r".���ң�Ĭ�ϣ�,"m".����,"l".����<br/>
					&emsp;&emsp;&emsp;&emsp;btn1Fn�� ѡ��������ť1��Ļص�������<br/>
					&emsp;&emsp;&emsp;&emsp;btn2Fn�� ѡ��������ť2��Ļص�������<br/>
				&emsp;&emsp;}</p>
			</li>
			<li>5. �ر���ʾ��
				<p>easyPoped.closeMsg(id): </p>
				<p>&emsp;&emsp;������Ҫ�رյ���ʾ���id����</p>
			</li>
			<li>6. �رյ������ڣ�
				<p>easyPoped.close(): </p>
				<p>&emsp;&emsp;ֱ�ӵ��ü��ɹرյ�ǰҳ��ĵ�������</p>
			</li>
		</ul>
		<h3>�����Ҫ�Զ�����ʽ������Ϊ��ʽ������ֱ���޸ļ���</h3>
		<ul>
			<li>1. easyUtil-poped-ShadeBody��
				<p>&emsp;&emsp;���ֲ���ʽ</p>
			</li>
			<li>2. easyUtil-poped-out��
				<p>&emsp;&emsp;�������ڻ�����ʽ</p>
			</li>
			<li>3. easyUtil-poped-title��
				<p>&emsp;&emsp;���������ʽ</p>
			</li>
			<li>4. easyUtil-poped-content��
				<p>&emsp;&emsp;���ݻ�����ʽ</p>
			</li>
			<li>5. easyUtil-poped-btns��
				<p>&emsp;&emsp;��ť�������ʽ</p>
			</li>
			<li>6. easyUtil-poped-btns-btn1/btn2��
				<p>&emsp;&emsp;������ť������ʽ</p>
			</li>
			<li>7. easyUtil-poped-Tips-out��
				<p>&emsp;&emsp;��ʾ�������ʽ</p>
			</li>
			<li>8. easyUtil-poped-Tips-in��
				<p>&emsp;&emsp;��ʾ���ڴ���ʽ</p>
			</li>
		</ul>
		<h4>����ΪAPI���ܣ���1.0�棬�Բ�IE10+,FF,Chrome����</h4>