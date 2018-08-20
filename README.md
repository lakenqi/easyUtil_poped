# easyUtil_poped
Modal Dialogue Box by  JavaScript
<h3>简介</h3>
		<h4>&emsp;&emsp;easyUtil.poped是简单的模态弹出窗口，拥有提示框，警告框，对话框以及弹出窗口功能，有两种颜色样式可以选择，也可以自定义样式，修改css文件对应类即可。</h4>
		<h4>&emsp;&emsp;easyUtil.poped支持模块化引用</h4>
		<h3>API:</h3>
		<h3>入口</h3>
		<ul>
			<li>1.普通调用全局引用名称为easyPoped，模块化可自定义名称</li>
			<li>2.保证easyUtilPoped_v1.0文件夹目录结构，并整体放到项目目录下，引用文件即可</li>
		</ul>
		<h3>具体方法及参数（以普通调用名称为例）</h3>
		<ul>
			<li>1. 提示框：
				<p>easyPoped.msg(text, time, offset): </p>
				<p>&emsp;&emsp;text： String或Number类型，提示内容； </p>
				<p>&emsp;&emsp;time：选填项 ,默认1000ms, Number类型，自动关闭时间 ms 设为0则手动关闭；如不设置此项，也可直接写offset偏移量</p>
				<p>&emsp;&emsp;offset：选填项， Array类型，弹出框偏移量top,left两个值，如只写一个值，则设置top偏移，支持多种单位和百分比，如果不写单位，默认px。</p>
				<p>&emsp;&emsp;方法返回值为当前提示框的id,如果手动关闭，则可以将id传入closeMsg方法，关闭提示框</p>
			</li>
			<li>2. 弹出窗口：
				<p>easyPoped.open(option): </p>
				<p>&emsp;&emsp;option = {<br/>
					&emsp;&emsp;&emsp;&emsp;title： 弹出窗口的标题；<br/>
					&emsp;&emsp;&emsp;&emsp;url： 弹出页面的url地址；<br/>
					&emsp;&emsp;&emsp;&emsp;space： 选填项，默认[50%，50%],数组类型，弹出层窗口宽高，如只写一个值，则设置width，支持多种单位和百分比，如果不写单位，默认px；<br/>
					&emsp;&emsp;&emsp;&emsp;style： 选填项，窗口样式，1.亮色（默认），2.暗色；<br/>
					&emsp;&emsp;&emsp;&emsp;closeBtn： 选填项，右上角关闭样式，1.黑色（默认），2.白色，如不需要，则填0；<br/>
					&emsp;&emsp;&emsp;&emsp;outClose： 选填项，点击遮罩层是否可以关闭，默认true，可关闭；<br/>
					&emsp;&emsp;&emsp;&emsp;closeFn： 选填项，关闭窗口后的回调函数；<br/>
				&emsp;&emsp;}</p>
			</li>
			<li>3. 警告框：
				<p>easyPoped.alert(option): </p>
				<p>&emsp;&emsp;option = {<br/>
					&emsp;&emsp;&emsp;&emsp;title： 警告窗口的标题；<br/>
					&emsp;&emsp;&emsp;&emsp;content：警告内容；<br/>
					&emsp;&emsp;&emsp;&emsp;icon： 选填项，提示图标,0无，1警告，2成功（默认），3失败，4询问；<br/>
					&emsp;&emsp;&emsp;&emsp;style： 选填项，窗口样式，1.亮色（默认），2.暗色；<br/>
					&emsp;&emsp;&emsp;&emsp;closeBtn： 选填项，右上角关闭样式，1.黑色（默认），2.白色，如不需要，则填0；<br/>
					&emsp;&emsp;&emsp;&emsp;outClose： 选填项，点击遮罩层是否可以关闭，默认false，不可关闭；<br/>
					&emsp;&emsp;&emsp;&emsp;btn: 选填项，数组类型，按钮的名称，默认"确定"；<br/>
					&emsp;&emsp;&emsp;&emsp;btnsRML: 按钮的位置，"r".居右（默认）,"m".居中,"l".居左；<br/>
					&emsp;&emsp;&emsp;&emsp;btnFn： 选填项，点击确认按钮后的回调函数；<br/>
				&emsp;&emsp;}</p>
			</li>
			<li>4. 确认框：
				<p>easyPoped.confirm(option): </p>
				<p>&emsp;&emsp;option = {<br/>
					&emsp;&emsp;&emsp;&emsp;title： 确认窗口的标题；<br/>
					&emsp;&emsp;&emsp;&emsp;content：确认内容；<br/>
					&emsp;&emsp;&emsp;&emsp;icon： 选填项，提示图标,0无，1警告，2成功，3失败，4询问（默认）；<br/>
					&emsp;&emsp;&emsp;&emsp;style： 选填项，窗口样式，1.亮色（默认），2.暗色；<br/>
					&emsp;&emsp;&emsp;&emsp;closeBtn： 选填项，右上角关闭样式，1.黑色（默认），2.白色，如不需要，则填0；<br/>
					&emsp;&emsp;&emsp;&emsp;outClose： 选填项，点击遮罩层是否可以关闭，默认false，不可关闭；<br/>
					&emsp;&emsp;&emsp;&emsp;btn1: 选填项，按钮1的名称，默认"确定"；<br/>
					&emsp;&emsp;&emsp;&emsp;btn2: 选填项，按钮2的名称，默认"取消"；<br/>
					&emsp;&emsp;&emsp;&emsp;btnsRML: 按钮的位置，"r".居右（默认）,"m".居中,"l".居左；<br/>
					&emsp;&emsp;&emsp;&emsp;btn1Fn： 选填项，点击按钮1后的回调函数；<br/>
					&emsp;&emsp;&emsp;&emsp;btn2Fn： 选填项，点击按钮2后的回调函数；<br/>
				&emsp;&emsp;}</p>
			</li>
			<li>5. 关闭提示框：
				<p>easyPoped.closeMsg(id): </p>
				<p>&emsp;&emsp;传入需要关闭的提示框的id即可</p>
			</li>
			<li>6. 关闭弹出窗口：
				<p>easyPoped.close(): </p>
				<p>&emsp;&emsp;直接调用即可关闭当前页面的弹出窗口</p>
			</li>
		</ul>
		<h3>如果需要自定义样式，以下为样式类名，直接修改即可</h3>
		<ul>
			<li>1. easyUtil-poped-ShadeBody：
				<p>&emsp;&emsp;遮罩层样式</p>
			</li>
			<li>2. easyUtil-poped-out：
				<p>&emsp;&emsp;弹出窗口基本样式</p>
			</li>
			<li>3. easyUtil-poped-title：
				<p>&emsp;&emsp;标题基本样式</p>
			</li>
			<li>4. easyUtil-poped-content：
				<p>&emsp;&emsp;内容基本样式</p>
			</li>
			<li>5. easyUtil-poped-btns：
				<p>&emsp;&emsp;按钮组基本样式</p>
			</li>
			<li>6. easyUtil-poped-btns-btn1/btn2：
				<p>&emsp;&emsp;单个按钮基本样式</p>
			</li>
			<li>7. easyUtil-poped-Tips-out：
				<p>&emsp;&emsp;提示框外层样式</p>
			</li>
			<li>8. easyUtil-poped-Tips-in：
				<p>&emsp;&emsp;提示框内存样式</p>
			</li>
		</ul>
		<h4>以上为API介绍，此1.0版，自测IE10+,FF,Chrome兼容</h4>