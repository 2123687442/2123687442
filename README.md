- 👋 Hi, I’m @2123687442
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
2123687442/2123687442 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<pre><code class="prism language-js"><span class="token keyword">var</span> name <span class="token operator">&#61;</span> <span class="token string">&#39;window&#39;</span>
<span class="token comment">// var name &#61; &#39;window&#39; 表示在window中name的值为 ’window‘</span>

<span class="token keyword">var</span> person <span class="token operator">&#61;</span> <span class="token punctuation">{<!-- --></span>
    <span class="token literal-property property">name</span><span class="token operator">:</span> <span class="token string">&#39;person&#39;</span><span class="token punctuation">,</span>
    <span class="token function-variable function">sayName</span><span class="token operator">:</span> <span class="token keyword">function</span> <span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{<!-- --></span>
        console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token keyword">this</span><span class="token punctuation">.</span>name<span class="token punctuation">)</span>
    <span class="token punctuation">}</span>
<span class="token punctuation">}</span>

<span class="token keyword">function</span> <span class="token function">sayName</span> <span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{<!-- --></span>
    <span class="token keyword">var</span> sss <span class="token operator">&#61;</span> person<span class="token punctuation">.</span>sayName<span class="token punctuation">;</span>

    <span class="token function">sss</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span><span class="token comment">// window  独立调用指向全局对象window</span>

    person<span class="token punctuation">.</span><span class="token function">sayName</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span> <span class="token comment">// person  隐式调用</span>

    <span class="token punctuation">(</span>person<span class="token punctuation">.</span>sayName<span class="token punctuation">)</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span> <span class="token comment">// person  和上一句效果一样(person.sayName) 带小括号不带小括号没区别</span>

    <span class="token punctuation">(</span>b <span class="token operator">&#61;</span> person<span class="token punctuation">.</span>sayName<span class="token punctuation">)</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token comment">// window  间接引用 &#xff0c;(b &#61; person.sayName)的结果是一个值&#xff0c;并没有和person对象有联系&#xff0c;所以后面加一个&#xff08;&#xff09;进行调用的时候&#xff0c;还是属于默认绑定&#xff08;直接调用&#xff09;&#xff0c;this指向全局对象</span>
<span class="token punctuation">}</span>

<span class="token function">sayName</span><span class="token punctuation">(</span><span class="token punctuation">)</span>
</code></pre> 
