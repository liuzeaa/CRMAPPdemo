#ejs安装 （ejs本事nodejs的一个模板，但是下载ejs.js包 ,也可以运行在浏览器上）

npm install ejs

# 调用  ejs.render(str, options); 第一个参数是 模板 的字符串，模板如下：

	<% if (names.length) { %>  
	  <ul>  
		<% names.forEach(function(name){ %>  
		  <li foo='<%= name + "'" %>'><%= name %></li>  
		<% }) %>  
	  </ul>  
	<% } %>  
（<% ... %> 写js代码，<%= ... %> 写字段参数）

#第二个参数是数据，一般是一个对象。而这个对象又可以视作为选项，也就是说数据和选择都在同一个对象身上。
