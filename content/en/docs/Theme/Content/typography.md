---
categories: ["Content"]
tags: ["typography", "style"]
title: "Typography"
linkTitle: "Typography"
date: 2022-01-18
description: >
  Typography plays an important role in creating an attractive and clear interface design. Good typography will make the content easy to follow and improve the usability of your website.
---


<div class="markdown">
                      <div>
                        <div class="d-flex mb-3">
                          <h1 class="m-0"></h1>
                          <p class="ms-auto">
                            <a href="https://getbootstrap.com/docs/5.0/content/typography/" target="_blank" class="d-flex align-items-center">
                              <!-- Download SVG icon from http://tabler-icons.io/i/external-link -->
                              <svg xmlns="http://www.w3.org/2000/svg" class="icon pe-1 text-blue" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><path d="M11 7h-5a2 2 0 0 0 -2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2 -2v-5"></path><line x1="10" y1="14" x2="20" y2="4"></line><polyline points="15 4 20 4 20 9"></polyline></svg>
                              Bootstrap documentation
                            </a>
                          </p>
                        </div>
                        <p>The Tabler theme is built on top of Bootstrap 5.0, so you can also utilize framework styles from the Bootstrap 5 documentation.</p>
                      </div>
                      <h2 id="headings">Headings</h2>
                      <p>Use HTML headings to organize content on your website and make the structure clear and user-friendly.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <h1>H1 Heading</h1>
                          <h2>H2 Heading</h2>
                          <h3>H3 Heading</h3>
                          <h4>H4 Heading</h4>
                          <h5>H5 Heading</h5>
                          <h6>H6 Heading</h6>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;h1&gt;</span>H1 Heading<span class="nt">&lt;/h1&gt;</span>
<span class="nt">&lt;h2&gt;</span>H2 Heading<span class="nt">&lt;/h2&gt;</span>
<span class="nt">&lt;h3&gt;</span>H3 Heading<span class="nt">&lt;/h3&gt;</span>
<span class="nt">&lt;h4&gt;</span>H4 Heading<span class="nt">&lt;/h4&gt;</span>
<span class="nt">&lt;h5&gt;</span>H5 Heading<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;h6&gt;</span>H6 Heading<span class="nt">&lt;/h6&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="paragraphs">Paragraphs</h2>
                      <p>Organize longer pieces of text into paragraphs using the <code class="language-plaintext highlighter-rouge">p</code> tag.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.</p>
                          <p>At vero eos et accusam et justo duo dolores et ea rebum.</p>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;p&gt;</span>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p&gt;</span>At vero eos et accusam et justo duo dolores et ea rebum.<span class="nt">&lt;/p&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="semantic-text-elements">Semantic text elements</h2>
                      <p>Use a variety of semantic text elements, depending of how you want to display particular fragments of content.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <abbr title="Internationalization">I18N</abbr> <code class="ms-2">abbr</code><br>
                          <strong>Bold</strong> <code class="ms-2">strong</code> <code>b</code><br>
                          <cite>Citation</cite> <code class="ms-2">cite</code><br>
                          <code>Hello World!</code> <code class="ms-2">code</code><br>
                          <del>Deleted</del> <code class="ms-2">del</code><br>
                          <em>Emphasis</em> <code class="ms-2">em</code><br>
                          <i>Italic</i> <code class="ms-2">i</code><br>
                          <ins>Inserted</ins> <code class="ms-2">ins</code><br>
                          <kbd>Ctrl + S</kbd> <code class="ms-2">kbd</code><br>
                          <mark>Highlighted</mark> <code class="ms-2">mark</code><br>
                          <s>Strikethrough</s> <code class="ms-2">s</code><br>
                          <samp>Sample</samp> <code class="ms-2">samp</code><br>
                          Text <sub>Subscripted</sub> <code class="ms-2">sub</code><br>
                          Text <sup>Superscripted</sup> <code class="ms-2">sup</code><br>
                          <time>20:00</time> <code class="ms-2">time</code><br>
                          <u>Underline</u> <code class="ms-2">u</code><br>
                          <var>x</var> = <var>y</var> + 2 <code class="ms-2">var</code><br>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;abbr</span> <span class="na">title=</span><span class="s">"Internationalization"</span><span class="nt">&gt;</span>I18N<span class="nt">&lt;/abbr&gt;</span>
<span class="nt">&lt;strong&gt;</span>Bold<span class="nt">&lt;/strong&gt;</span>
<span class="nt">&lt;cite&gt;</span>Citation<span class="nt">&lt;/cite&gt;</span>
<span class="nt">&lt;code&gt;</span>Hello World!<span class="nt">&lt;/code&gt;</span>
<span class="nt">&lt;del&gt;</span>Deleted<span class="nt">&lt;/del&gt;</span>
<span class="nt">&lt;em&gt;</span>Emphasis<span class="nt">&lt;/em&gt;</span>
<span class="nt">&lt;i&gt;</span>Italic<span class="nt">&lt;/i&gt;</span>
<span class="nt">&lt;ins&gt;</span>Inserted<span class="nt">&lt;/ins&gt;</span>
<span class="nt">&lt;kbd&gt;</span>Ctrl + S<span class="nt">&lt;/kbd&gt;</span>
<span class="nt">&lt;mark&gt;</span>Highlighted<span class="nt">&lt;/mark&gt;</span>
<span class="nt">&lt;s&gt;</span>Strikethrough<span class="nt">&lt;/s</span>
<span class="err">&lt;samp</span><span class="nt">&gt;</span>Sample<span class="nt">&lt;/samp&gt;</span>
Text <span class="nt">&lt;sub&gt;</span>Subscripted<span class="nt">&lt;/sub&gt;</span>
Text <span class="nt">&lt;sup&gt;</span>Superscripted<span class="nt">&lt;/sup&gt;</span>
<span class="nt">&lt;time&gt;</span>20:00<span class="nt">&lt;/time&gt;</span>
<span class="nt">&lt;u&gt;</span>Underline<span class="nt">&lt;/u&gt;</span>
<span class="nt">&lt;var&gt;</span>x<span class="nt">&lt;/var&gt;</span> = <span class="nt">&lt;var&gt;</span>y<span class="nt">&lt;/var&gt;</span> + 2</code></pre>
                        </figure>
                      </div>
                      <h2 id="horizontal-rules">Horizontal rules</h2>
                      <p>Use the <code class="language-plaintext highlighter-rouge">hr</code> tag to represent a thematic break between paragraphs within one section.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <hr>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;hr&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="horizontal-rules-with-label">Horizontal rules with label</h2>
                      <p>You can also add a label to a horizontal rule and align it as you see fit.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <p>
                            Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.
                          </p>
                          <div class="hr-text">
                            <span>Rule text</span>
                          </div>
                          <p>
                            At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
                          </p>
                          <div class="hr-text hr-text-center">
                            <span>Rule text</span>
                          </div>
                          <p>
                            Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.
                          </p>
                          <div class="hr-text hr-text-end">
                            <span>Rule text</span>
                          </div>
                          <p>
                            At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
                          </p>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;p&gt;</span>
  Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.
<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"hr-text"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;span&gt;</span>Rule text<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;p&gt;</span>
  At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"hr-text hr-text-center"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;span&gt;</span>Rule text<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;p&gt;</span>
  Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.
<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"hr-text hr-text-end"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;span&gt;</span>Rule text<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;p&gt;</span>
  At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
<span class="nt">&lt;/p&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="optimized-for-different-alphabets">Optimized for different alphabets</h2>
                      <p>Tabler has been optimized to correctly display content in any language. It supports most Asian, African and Middle Eastern languages.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <h5>Chinese</h5>
                          <p>汉字</p>
                          <h5>Japanese</h5>
                          <p>日本語の表記体系</p>
                          <h5>Korean</h5>
                          <p>한글</p>
                          <h5>Cyrillic</h5>
                          <p>Кириллица</p>
                          <h5>Greek</h5>
                          <p>Eλληνική</p>
                          <h5>Georgian</h5>
                          <p>ქართული დამწერლობა</p>
                          <h5>Armenian</h5>
                          <p>Հայերենի այբուբեն</p>
                          <h5>Arabic</h5>
                          <p>الحروف العربية</p>
                          <h5>Hebrew</h5>
                          <p>אלפבית עברי</p>
                          <h5>Thai</h5>
                          <p>อักษรไทย</p>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;h5&gt;</span>Chinese<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>汉字<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Japanese<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>日本語の表記体系<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Korean<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>한글<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Cyrillic<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>Кириллица<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Greek<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>Eλληνική<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Georgian<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>ქართული დამწერლობა<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Armenian<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>Հայերենի այբուբեն<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Arabic<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>الحروف العربية<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Hebrew<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>אלפבית עברי<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;h5&gt;</span>Thai<span class="nt">&lt;/h5&gt;</span>
<span class="nt">&lt;p&gt;</span>อักษรไทย<span class="nt">&lt;/p&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="text-transform">Text transform</h2>
                      <p>Transform the content of components with text capitalization classes.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <p class="text-lowercase">Lowercased text.</p>
                          <p class="text-uppercase">Uppercased text.</p>
                          <p class="text-capitalize">Capitalized text.</p>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"text-lowercase"</span><span class="nt">&gt;</span>Lowercased text.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"text-uppercase"</span><span class="nt">&gt;</span>Uppercased text.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"text-capitalize"</span><span class="nt">&gt;</span>Capitalized text.<span class="nt">&lt;/p&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="letter-spacing">Letter spacing</h2>
                      <p>Control the tracking (letter spacing) of an element and make it tight, wide or normal.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <p class="tracking-tight">Lorem ipsum dolor sit amet. Tight letter spacing.</p>
                          <p class="tracking-normal">Lorem ipsum dolor sit amet. Normal letter spacing.</p>
                          <p class="tracking-wide">Lorem ipsum dolor sit amet. Wide letter spacing.</p>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"tracking-tight"</span><span class="nt">&gt;</span>Lorem ipsum dolor sit amet. Tight letter spacing.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"tracking-normal"</span><span class="nt">&gt;</span>Lorem ipsum dolor sit amet. Normal letter spacing.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"tracking-wide"</span><span class="nt">&gt;</span>Lorem ipsum dolor sit amet. Wide letter spacing.<span class="nt">&lt;/p&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="line-height">Line height</h2>
                      <p>Control the leading (line height) of an element.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <p class="lh-1">Lorem ipsum dolor sit amet.<br>
                            Dolor sit amet.</p>
                          <p class="lh-sm">Lorem ipsum dolor sit amet.<br>
                            Dolor sit amet.</p>
                          <p class="lh-base">Lorem ipsum dolor sit amet.<br>
                            Dolor sit amet.</p>
                          <p class="lh-lg">Lorem ipsum dolor sit amet.<br>
                            Dolor sit amet.</p>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"lh-1"</span><span class="nt">&gt;</span>Lorem ipsum dolor sit amet.<span class="nt">&lt;br&gt;</span>
  Dolor sit amet.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"lh-sm"</span><span class="nt">&gt;</span>Lorem ipsum dolor sit amet.<span class="nt">&lt;br&gt;</span>
  Dolor sit amet.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"lh-base"</span><span class="nt">&gt;</span>Lorem ipsum dolor sit amet.<span class="nt">&lt;br&gt;</span>
  Dolor sit amet.<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"lh-lg"</span><span class="nt">&gt;</span>Lorem ipsum dolor sit amet.<span class="nt">&lt;br&gt;</span>
  Dolor sit amet.<span class="nt">&lt;/p&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="antialiasing">Antialiasing</h2>
                      <p>Control the font smoothing of an element.</p>
                      <p>Use the <code class="language-plaintext highlighter-rouge">.antialiased</code> utility to render text using subpixel antialiasing or use the <code class="language-plaintext highlighter-rouge">.subpixel-antialiased</code> utility to remove antialiasing.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="antialiased">Text with antialiasing</div>
                          <div class="subpixel-antialiased">Text without antialiasing</div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"antialiased"</span><span class="nt">&gt;</span>Text with antialiasing<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"subpixel-antialiased"</span><span class="nt">&gt;</span>Text without antialiasing<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="markdown-elements">Markdown elements</h2>
                      <p>If you can’t use the CSS classes you want or if you just want to use HTML tags, use the <code class="language-plaintext highlighter-rouge">.markdown</code> class in a container. It can handle almost any HTML tag.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="markdown">
                            <h1>Hello World</h1>
                            <p>Lorem ipsum<sup><a>[1]</a></sup> dolor sit amet, consectetur adipiscing elit. Nulla accumsan, metus ultrices eleifend gravida, nulla nunc varius lectus, nec rutrum justo nibh eu lectus. Ut vulputate semper dui. Fusce erat odio, sollicitudin vel erat vel, interdum mattis neque. Sub<sub>script</sub> works as well!</p>
                            <h2>Second level</h2>
                            <p>Curabitur accumsan turpis pharetra <strong>augue tincidunt</strong> blandit. Quisque condimentum maximus mi, sit amet commodo arcu rutrum id. Proin pretium urna vel cursus venenatis. Suspendisse potenti. Etiam mattis sem rhoncus lacus dapibus facilisis. Donec at dignissim dui. Ut et neque nisl.</p>
                            <ul>
                              <li>In fermentum leo eu lectus mollis, quis dictum mi aliquet.</li>
                              <li>Morbi eu nulla lobortis, lobortis est in, fringilla felis.</li>
                              <li>Aliquam nec felis in sapien venenatis viverra fermentum nec lectus.</li>
                              <li>Ut non enim metus.</li>
                            </ul>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"markdown"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;h1&gt;</span>Hello World<span class="nt">&lt;/h1&gt;</span>
  <span class="nt">&lt;p&gt;</span>Lorem ipsum<span class="nt">&lt;sup&gt;&lt;a&gt;</span>[1]<span class="nt">&lt;/a&gt;&lt;/sup&gt;</span> dolor sit amet, consectetur adipiscing elit. Nulla accumsan, metus ultrices eleifend gravida, nulla nunc varius lectus, nec rutrum justo nibh eu lectus. Ut vulputate semper dui. Fusce erat odio, sollicitudin vel erat vel, interdum mattis neque. Sub<span class="nt">&lt;sub&gt;</span>script<span class="nt">&lt;/sub&gt;</span> works as well!<span class="nt">&lt;/p&gt;</span>
  <span class="nt">&lt;h2&gt;</span>Second level<span class="nt">&lt;/h2&gt;</span>
  <span class="nt">&lt;p&gt;</span>Curabitur accumsan turpis pharetra <span class="nt">&lt;strong&gt;</span>augue tincidunt<span class="nt">&lt;/strong&gt;</span> blandit. Quisque condimentum maximus mi, sit amet commodo arcu rutrum id. Proin pretium urna vel cursus venenatis. Suspendisse potenti. Etiam mattis sem rhoncus lacus dapibus facilisis. Donec at dignissim dui. Ut et neque nisl.<span class="nt">&lt;/p&gt;</span>
  <span class="nt">&lt;ul&gt;</span>
    <span class="nt">&lt;li&gt;</span>In fermentum leo eu lectus mollis, quis dictum mi aliquet.<span class="nt">&lt;/li&gt;</span>
    <span class="nt">&lt;li&gt;</span>Morbi eu nulla lobortis, lobortis est in, fringilla felis.<span class="nt">&lt;/li&gt;</span>
    <span class="nt">&lt;li&gt;</span>Aliquam nec felis in sapien venenatis viverra fermentum nec lectus.<span class="nt">&lt;/li&gt;</span>
    <span class="nt">&lt;li&gt;</span>Ut non enim metus.<span class="nt">&lt;/li&gt;</span>
  <span class="nt">&lt;/ul&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                    </div>