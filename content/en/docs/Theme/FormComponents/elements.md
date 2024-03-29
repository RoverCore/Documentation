---
title: "Form Elements"
linkTitle: "Form Elements"
date: 2022-01-18
description: >
  Forms are one of the most important types of interaction with a website or app. Since their aim is to enable users to make a purchase, subscribe to a service or sign up to create an account, it's important to make sure they are easy to complete and help increase conversion rates. Use the available elements to create forms which are well-structured and user-friendly.
---

<div class="markdown">
                      <div>
                        <div class="d-flex mb-3">
                          <p class="ms-auto">
                            <a href="https://getbootstrap.com/docs/5.0/components/forms/" target="_blank" class="d-flex align-items-center">
                              <!-- Download SVG icon from http://tabler-icons.io/i/external-link -->
                              <svg xmlns="http://www.w3.org/2000/svg" class="icon pe-1 text-blue" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><path d="M11 7h-5a2 2 0 0 0 -2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2 -2v-5"></path><line x1="10" y1="14" x2="20" y2="4"></line><polyline points="15 4 20 4 20 9"></polyline></svg>
                              Bootstrap documentation
                            </a>
                          </p>
                        </div>
                      </div>
                      <h2 id="classic-inputs">Classic inputs</h2>
                      <p>Use classic, user-friendly inputs, label them appropriately and include input placeholders that will help users avoid confusion when completing a form.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Text</label>
                            <input type="text" class="form-control" name="example-text-input" placeholder="Input placeholder">
                          </div>
                          <div class="mb-3">
                            <label class="form-label">Password</label>
                            <input type="text" class="form-control" name="example-password-input" placeholder="Input placeholder">
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Text<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">name=</span><span class="s">"example-text-input"</span> <span class="na">placeholder=</span><span class="s">"Input placeholder"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Password<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">name=</span><span class="s">"example-password-input"</span> <span class="na">placeholder=</span><span class="s">"Input placeholder"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="form-control-rounded">Form control rounded</h2>
                      <p>Use the <code class="language-plaintext highlighter-rouge">form-control-rounded</code> class if you prefer form controls with rounded corners.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Form control rounded</label>
                            <input type="text" class="form-control form-control-rounded mb-2" name="Form control rounded" placeholder="Text..">
                            <div class="input-icon">
                              <input type="text" class="form-control form-control-rounded" placeholder="Search…">
                              <span class="input-icon-addon">
                                <!-- Download SVG icon from http://tabler-icons.io/i/search -->
                                <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><circle cx="10" cy="10" r="7"></circle><line x1="21" y1="21" x2="15" y2="15"></line></svg>
                              </span>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Form control rounded<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control form-control-rounded mb-2"</span> <span class="na">name=</span><span class="s">"Form control rounded"</span> <span class="na">placeholder=</span><span class="s">"Text.."</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-icon"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control form-control-rounded"</span> <span class="na">placeholder=</span><span class="s">"Search…"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-icon-addon"</span><span class="nt">&gt;</span>
      <span class="c">&lt;!-- Download SVG icon from http://tabler-icons.io/i/search --&gt;</span>
      <span class="c">&lt;!-- SVG icon code --&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="form-control-flush">Form control flush</h2>
                      <p>You can remove borders from your form control by adding the <code class="language-plaintext highlighter-rouge">form-control-flush</code> class.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Form control flush</label>
                            <input type="text" class="form-control form-control-flush" name="Form control flush" placeholder="Text..">
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Form control flush<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control form-control-flush"</span> <span class="na">name=</span><span class="s">"Form control flush"</span> <span class="na">placeholder=</span><span class="s">"Text.."</span><span class="nt">&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="input-with-icon">Input with icon</h2>
                      <p>Add icons to your input controls to suggest users what they should enter or inform them of the current state of a form element.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Icon input</label>
                            <div class="input-icon mb-3">
                              <input type="text" class="form-control" placeholder="Search…">
                              <span class="input-icon-addon">
                                <!-- Download SVG icon from http://tabler-icons.io/i/search -->
                                <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><circle cx="10" cy="10" r="7"></circle><line x1="21" y1="21" x2="15" y2="15"></line></svg>
                              </span>
                            </div>
                            <div class="input-icon mb-3">
                              <span class="input-icon-addon">
                                <!-- Download SVG icon from http://tabler-icons.io/i/user -->
                                <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><circle cx="12" cy="7" r="4"></circle><path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2"></path></svg>
                              </span>
                              <input type="text" class="form-control" placeholder="Username">
                            </div>
                          </div>
                          <div class="mb-3">
                            <label class="form-label">Loader input</label>
                            <div class="input-icon mb-3">
                              <input type="text" class="form-control" placeholder="Loading…">
                              <span class="input-icon-addon">
                                <div class="spinner-border spinner-border-sm text-muted" role="status"></div>
                              </span>
                            </div>
                            <div class="input-icon mb-3">
                              <span class="input-icon-addon">
                                <div class="spinner-border spinner-border-sm text-muted" role="status"></div>
                              </span>
                              <input type="text" class="form-control" placeholder="Loading…">
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Icon input<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-icon mb-3"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">placeholder=</span><span class="s">"Search…"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-icon-addon"</span><span class="nt">&gt;</span>
      <span class="c">&lt;!-- Download SVG icon from http://tabler-icons.io/i/search --&gt;</span>
      <span class="c">&lt;!-- SVG icon code --&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-icon mb-3"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-icon-addon"</span><span class="nt">&gt;</span>
      <span class="c">&lt;!-- Download SVG icon from http://tabler-icons.io/i/user --&gt;</span>
      <span class="c">&lt;!-- SVG icon code --&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">placeholder=</span><span class="s">"Username"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Loader input<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-icon mb-3"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">placeholder=</span><span class="s">"Loading…"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-icon-addon"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"spinner-border spinner-border-sm text-muted"</span> <span class="na">role=</span><span class="s">"status"</span><span class="nt">&gt;&lt;/div&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-icon mb-3"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-icon-addon"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"spinner-border spinner-border-sm text-muted"</span> <span class="na">role=</span><span class="s">"status"</span><span class="nt">&gt;&lt;/div&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">placeholder=</span><span class="s">"Loading…"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="separated-inputs">Separated inputs</h2>
                      <p>Include an additional element in your input section, such as a button which can be used to submit the information enetered in the input control.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Separated inputs</label>
                            <div class="row g-2">
                              <div class="col">
                                <input type="text" class="form-control" placeholder="Search for…">
                              </div>
                              <div class="col-auto">
                                <a href="javascript:void(0)" class="btn btn-white btn-icon" aria-label="Button">
                                  <!-- Download SVG icon from http://tabler-icons.io/i/search -->
                                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><circle cx="10" cy="10" r="7"></circle><line x1="21" y1="21" x2="15" y2="15"></line></svg>
                                </a>
                              </div>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Separated inputs<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"row g-2"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"col"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">placeholder=</span><span class="s">"Search for…"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/div&gt;</span>
    <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"col-auto"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"#"</span> <span class="na">class=</span><span class="s">"btn btn-white btn-icon"</span> <span class="na">aria-label=</span><span class="s">"Button"</span><span class="nt">&gt;</span>
        <span class="c">&lt;!-- Download SVG icon from http://tabler-icons.io/i/search --&gt;</span>
        <span class="c">&lt;!-- SVG icon code --&gt;</span>
      <span class="nt">&lt;/a&gt;</span>
    <span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="textarea-and-select">Textarea and select</h2>
                      <p>Use a multi-line text input control to enable users to enter longer pieces of text. The control will automatically adjust to the length of the text entered.</p>
                      <p>Add one of the available selects - either a dropdown or a multiple choice select - to let users choose from a predefined set of options.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Textarea</label>
                            <textarea class="form-control" name="example-textarea" placeholder="Textarea placeholder"></textarea>
                          </div>
                          <div class="mb-3">
                            <div class="form-label">Select</div>
                            <select class="form-select">
                              <option value="1">One</option>
                              <option value="2">Two</option>
                              <option value="3">Three</option>
                            </select>
                          </div>
                          <div class="mb-3">
                            <div class="form-label">Select multiple</div>
                            <select class="form-select" multiple="">
                              <option value="1">One</option>
                              <option value="2">Two</option>
                              <option value="3">Three</option>
                            </select>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Textarea<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;textarea</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">name=</span><span class="s">"example-textarea"</span> <span class="na">placeholder=</span><span class="s">"Textarea placeholder"</span><span class="nt">&gt;&lt;/textarea&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Select<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;select</span> <span class="na">class=</span><span class="s">"form-select"</span> <span class="nt">&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"1"</span><span class="nt">&gt;</span>One<span class="nt">&lt;/option&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"2"</span><span class="nt">&gt;</span>Two<span class="nt">&lt;/option&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"3"</span><span class="nt">&gt;</span>Three<span class="nt">&lt;/option&gt;</span>
  <span class="nt">&lt;/select&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Select multiple<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;select</span> <span class="na">class=</span><span class="s">"form-select"</span>  <span class="na">multiple</span><span class="nt">&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"1"</span><span class="nt">&gt;</span>One<span class="nt">&lt;/option&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"2"</span><span class="nt">&gt;</span>Two<span class="nt">&lt;/option&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"3"</span><span class="nt">&gt;</span>Three<span class="nt">&lt;/option&gt;</span>
  <span class="nt">&lt;/select&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="input-size">Input size</h2>
                      <p>Choose the size of an input control that will go well with your form design. Apart from the default size, you can also use small and large input controls.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Input sizing</label>
                            <input class="form-control form-control-lg mb-2" type="text" placeholder=".form-control-lg">
                            <input class="form-control mb-2" type="text" placeholder="Default input">
                            <input class="form-control form-control-sm" type="text" placeholder=".form-control-sm">
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Input sizing<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-control form-control-lg mb-2"</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">placeholder=</span><span class="s">".form-control-lg"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-control mb-2"</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">placeholder=</span><span class="s">"Default input"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-control form-control-sm"</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">placeholder=</span><span class="s">".form-control-sm"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="datalists">Datalists</h2>
                      <p>Use the <code class="language-plaintext highlighter-rouge">datalist</code> element to add an autocomplete feature to your input control. The list of available options will display once a user starts to type and will make it quicker to complete form sections.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Datalist example</label>
                            <input class="form-control" list="datalistOptions" placeholder="Type to search...">
                            <datalist id="datalistOptions">
                              <option value="Aruba">
                              </option><option value="Afghanistan">
                              </option><option value="Angola">
                              </option><option value="Anguilla">
                              </option><option value="Albania">
                              </option><option value="Andorra">
                              </option><option value="United Arab Emirates">
                              </option><option value="Argentina">
                              </option><option value="Armenia">
                              </option><option value="American Samoa">
                            </option></datalist>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Datalist example<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-control"</span> <span class="na">list=</span><span class="s">"datalistOptions"</span> <span class="na">placeholder=</span><span class="s">"Type to search..."</span><span class="nt">/&gt;</span>
  <span class="nt">&lt;datalist</span> <span class="na">id=</span><span class="s">"datalistOptions"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Aruba"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Afghanistan"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Angola"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Anguilla"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Albania"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Andorra"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"United Arab Emirates"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Argentina"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"Armenia"</span><span class="nt">/&gt;</span>
    <span class="nt">&lt;option</span> <span class="na">value=</span><span class="s">"American Samoa"</span><span class="nt">/&gt;</span>
  <span class="nt">&lt;/datalist&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="toggle-switches">Toggle switches</h2>
                      <p>Use toggle switches for the elements of your form which require choosing between two opposing states.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <div class="form-label">Toggle switches</div>
                            <label class="form-check form-switch">
                              <input class="form-check-input" type="checkbox" checked="">
                              <span class="form-check-label">Option 1</span>
                            </label>
                            <label class="form-check form-switch">
                              <input class="form-check-input" type="checkbox">
                              <span class="form-check-label">Option 2</span>
                            </label>
                            <label class="form-check form-switch">
                              <input class="form-check-input" type="checkbox">
                              <span class="form-check-label">Option 3</span>
                            </label>
                          </div>
                          <div class="mb-3">
                            <div class="form-label">Single switch</div>
                            <label class="form-check form-switch">
                              <input class="form-check-input" type="checkbox">
                              <span class="form-check-label">I agree with terms and conditions</span>
                            </label>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Toggle switches<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-switch"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span> <span class="na">checked</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 1<span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-switch"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 2<span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-switch"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 3<span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/label&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Single switch<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-switch"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>I agree with terms and conditions<span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/label&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="radios">Radios</h2>
                      <p>Use radio buttons for the parts of your form which require users to choose one option from a set of two or more mutually exclusive options.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <div class="form-label">Radios</div>
                            <div>
                              <label class="form-check">
                                <input class="form-check-input" type="radio" checked="">
                                <span class="form-check-label">Option 1</span>
                              </label>
                              <label class="form-check">
                                <input class="form-check-input" type="radio">
                                <span class="form-check-label">Option 2</span>
                              </label>
                              <label class="form-check">
                                <input class="form-check-input" type="radio" disabled="">
                                <span class="form-check-label">Option 3</span>
                              </label>
                              <label class="form-check">
                                <input class="form-check-input" type="radio" checked="" disabled="">
                                <span class="form-check-label">Option 4</span>
                              </label>
                            </div>
                          </div>
                          <div class="mb-3">
                            <div class="form-label">Inline Radios</div>
                            <div>
                              <label class="form-check form-check-inline">
                                <input class="form-check-input" type="radio" checked="">
                                <span class="form-check-label">Option 1</span>
                              </label>
                              <label class="form-check form-check-inline">
                                <input class="form-check-input" type="radio">
                                <span class="form-check-label">Option 2</span>
                              </label>
                              <label class="form-check form-check-inline">
                                <input class="form-check-input" type="radio" disabled="">
                                <span class="form-check-label">Option 3</span>
                              </label>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Radios<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"radio"</span> <span class="na">checked</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 1<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"radio"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 2<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"radio"</span> <span class="na">disabled</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 3<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"radio"</span> <span class="na">checked</span> <span class="na">disabled</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 4<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Inline Radios<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-check-inline"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"radio"</span> <span class="na">checked</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 1<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-check-inline"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"radio"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 2<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-check-inline"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"radio"</span> <span class="na">disabled</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 3<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="checkboxes">Checkboxes</h2>
                      <p>Use checkoxes if you want to allow users to select more than one option from a set of predefined options or to turn an option on or off.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <div class="form-label">Checkboxes</div>
                            <div>
                              <label class="form-check">
                                <input class="form-check-input" type="checkbox">
                                <span class="form-check-label">Checkbox input</span>
                              </label>
                              <label class="form-check">
                                <input class="form-check-input" type="checkbox" disabled="">
                                <span class="form-check-label">Disabled checkbox input</span>
                              </label>
                              <label class="form-check">
                                <input class="form-check-input" type="checkbox" checked="">
                                <span class="form-check-label">Checked checkbox input</span>
                              </label>
                            </div>
                          </div>
                          <div class="mb-3">
                            <div class="form-label">Inline Checkboxes</div>
                            <div>
                              <label class="form-check form-check-inline">
                                <input class="form-check-input" type="checkbox">
                                <span class="form-check-label">Option 1</span>
                              </label>
                              <label class="form-check form-check-inline">
                                <input class="form-check-input" type="checkbox" disabled="">
                                <span class="form-check-label">Option 2</span>
                              </label>
                              <label class="form-check form-check-inline">
                                <input class="form-check-input" type="checkbox" checked="">
                                <span class="form-check-label">Option 3</span>
                              </label>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Checkboxes<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Checkbox input<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span> <span class="na">disabled</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Disabled checkbox input<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span> <span class="na">checked</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Checked checkbox input<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Inline Checkboxes<span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-check-inline"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 1<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-check-inline"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span> <span class="na">disabled</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 2<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
    <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-check form-check-inline"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input"</span> <span class="na">type=</span><span class="s">"checkbox"</span> <span class="na">checked</span><span class="nt">&gt;</span>
      <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"form-check-label"</span><span class="nt">&gt;</span>Option 3<span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="range-input">Range input</h2>
                      <p>Add a range slider to make it possible for users to set a value or range, such as a price range or a time frame.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Range input</label>
                            <input type="range" class="form-range mb-2" value="40" min="0" max="100" step="10">
                            <div class="form-range mb-2 noUi-target noUi-ltr noUi-horizontal noUi-txt-dir-ltr" id="range-simple"><div class="noUi-base"><div class="noUi-connects"><div class="noUi-connect" style="transform: translate(0%, 0px) scale(0.2, 1);"></div></div><div class="noUi-origin" style="transform: translate(-80%, 0px); z-index: 4;"><div class="noUi-handle noUi-handle-lower" data-handle="0" tabindex="0" role="slider" aria-orientation="horizontal" aria-valuemin="0.0" aria-valuemax="100.0" aria-valuenow="20.0" aria-valuetext="20.00"><div class="noUi-touch-area"></div></div></div></div></div>
                            <div class="form-range mb-2 noUi-target noUi-ltr noUi-horizontal noUi-txt-dir-ltr" id="range-connect"><div class="noUi-base"><div class="noUi-connects"><div class="noUi-connect" style="transform: translate(60%, 0px) scale(0.3, 1);"></div></div><div class="noUi-origin" style="transform: translate(-40%, 0px); z-index: 5;"><div class="noUi-handle noUi-handle-lower" data-handle="0" tabindex="0" role="slider" aria-orientation="horizontal" aria-valuemin="0.0" aria-valuemax="90.0" aria-valuenow="60.0" aria-valuetext="60.00"><div class="noUi-touch-area"></div></div></div><div class="noUi-origin" style="transform: translate(-10%, 0px); z-index: 4;"><div class="noUi-handle noUi-handle-upper" data-handle="1" tabindex="0" role="slider" aria-orientation="horizontal" aria-valuemin="60.0" aria-valuemax="100.0" aria-valuenow="90.0" aria-valuetext="90.00"><div class="noUi-touch-area"></div></div></div></div></div>
                            <div class="form-range mb-2 text-green noUi-target noUi-ltr noUi-horizontal noUi-txt-dir-ltr" id="range-color"><div class="noUi-base"><div class="noUi-connects"><div class="noUi-connect" style="transform: translate(0%, 0px) scale(0.4, 1);"></div></div><div class="noUi-origin" style="transform: translate(-60%, 0px); z-index: 4;"><div class="noUi-handle noUi-handle-lower" data-handle="0" tabindex="0" role="slider" aria-orientation="horizontal" aria-valuemin="0.0" aria-valuemax="100.0" aria-valuenow="40.0" aria-valuetext="40.00"><div class="noUi-touch-area"></div></div></div></div></div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Range input<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"range"</span> <span class="na">class=</span><span class="s">"form-range mb-2"</span> <span class="na">value=</span><span class="s">"40"</span> <span class="na">min=</span><span class="s">"0"</span> <span class="na">max=</span><span class="s">"100"</span> <span class="na">step=</span><span class="s">"10"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-range mb-2"</span> <span class="na">id=</span><span class="s">"range-simple"</span><span class="nt">&gt;&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-range mb-2"</span> <span class="na">id=</span><span class="s">"range-connect"</span><span class="nt">&gt;&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"form-range mb-2 text-green"</span> <span class="na">id=</span><span class="s">"range-color"</span><span class="nt">&gt;&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;script&gt;</span>
  <span class="nx">noUiSlider</span><span class="p">.</span><span class="nx">create</span><span class="p">(</span><span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="dl">'</span><span class="s1">range-color</span><span class="dl">'</span><span class="p">),</span> <span class="p">{</span>
  	<span class="na">start</span><span class="p">:</span> <span class="mi">40</span><span class="p">,</span>
  	<span class="na">connect</span><span class="p">:</span> <span class="p">[</span><span class="kc">true</span><span class="p">,</span> <span class="kc">false</span><span class="p">],</span>
  	<span class="na">step</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
  	<span class="na">range</span><span class="p">:</span> <span class="p">{</span>
  		<span class="na">min</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
  		<span class="na">max</span><span class="p">:</span> <span class="mi">100</span>
  	<span class="p">}</span>
  <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="input-group">Input group</h2>
                      <p>Create a group of input controls and place add-ons on either side of an input.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Input group</label>
                            <div class="input-group mb-2">
                              <span class="input-group-text">
                                @
                              </span>
                              <input type="text" class="form-control" placeholder="username" autocomplete="off">
                            </div>
                            <div class="input-group mb-2">
                              <input type="text" class="form-control" placeholder="subdomain" autocomplete="off">
                              <span class="input-group-text">
                                .tabler.io
                              </span>
                            </div>
                            <div class="input-group">
                              <span class="input-group-text">
                                https://
                              </span>
                              <input type="text" class="form-control" placeholder="subdomain" autocomplete="off">
                              <span class="input-group-text">
                                .tabler.io
                              </span>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Input group<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group mb-2"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      @
    <span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span>  <span class="na">placeholder=</span><span class="s">"username"</span>  <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group mb-2"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span>  <span class="na">placeholder=</span><span class="s">"subdomain"</span>  <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      .tabler.io
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      https://
    <span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span>  <span class="na">placeholder=</span><span class="s">"subdomain"</span>  <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      .tabler.io
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;script&gt;</span>
  <span class="nx">noUiSlider</span><span class="p">.</span><span class="nx">create</span><span class="p">(</span><span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="dl">'</span><span class="s1">range-color</span><span class="dl">'</span><span class="p">),</span> <span class="p">{</span>
  	<span class="na">start</span><span class="p">:</span> <span class="mi">40</span><span class="p">,</span>
  	<span class="na">connect</span><span class="p">:</span> <span class="p">[</span><span class="kc">true</span><span class="p">,</span> <span class="kc">false</span><span class="p">],</span>
  	<span class="na">step</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
  	<span class="na">range</span><span class="p">:</span> <span class="p">{</span>
  		<span class="na">min</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
  		<span class="na">max</span><span class="p">:</span> <span class="mi">100</span>
  	<span class="p">}</span>
  <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="input-with-checkboxes-or-radios">Input with checkboxes or radios</h2>
                      <p>Add checkboxes or radio buttons on either side of your input control.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Input with checkbox or radios</label>
                            <div class="input-group mb-2">
                              <span class="input-group-text">
                                <input class="form-check-input m-0" type="checkbox" checked="">
                              </span>
                              <input type="text" class="form-control" autocomplete="off">
                            </div>
                            <div class="input-group">
                              <input type="text" class="form-control" autocomplete="off">
                              <span class="input-group-text">
                                <input class="form-check-input m-0" type="radio" checked="">
                              </span>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Input with checkbox or radios<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group mb-2"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input m-0"</span> <span class="na">type=</span><span class="s">"checkbox"</span> <span class="na">checked</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span>  <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span>  <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;input</span> <span class="na">class=</span><span class="s">"form-check-input m-0"</span> <span class="na">type=</span><span class="s">"radio"</span> <span class="na">checked</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;script&gt;</span>
  <span class="nx">noUiSlider</span><span class="p">.</span><span class="nx">create</span><span class="p">(</span><span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="dl">'</span><span class="s1">range-color</span><span class="dl">'</span><span class="p">),</span> <span class="p">{</span>
  	<span class="na">start</span><span class="p">:</span> <span class="mi">40</span><span class="p">,</span>
  	<span class="na">connect</span><span class="p">:</span> <span class="p">[</span><span class="kc">true</span><span class="p">,</span> <span class="kc">false</span><span class="p">],</span>
  	<span class="na">step</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
  	<span class="na">range</span><span class="p">:</span> <span class="p">{</span>
  		<span class="na">min</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
  		<span class="na">max</span><span class="p">:</span> <span class="mi">100</span>
  	<span class="p">}</span>
  <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="input-with-prepended-or-appended-text">Input with prepended or appended text</h2>
                      <p>Add text to your input control, either before or after the text which is to be entered by a user.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Input with prepended text</label>
                            <div class="input-group input-group-flat mb-2">
                              <span class="input-group-text">
                                https://tabler.io/users/
                              </span>
                              <input type="text" class="form-control ps-0" value="yourfancyusername" autocomplete="off">
                            </div>
                            <div class="input-group input-group-flat">
                              <input type="text" class="form-control text-end pe-0" value="yourfancydomain" autocomplete="off">
                              <span class="input-group-text">
                                .tabler.io
                              </span>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Input with prepended text<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group input-group-flat mb-2"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      https://tabler.io/users/
    <span class="nt">&lt;/span&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control ps-0"</span>  <span class="na">value=</span><span class="s">"yourfancyusername"</span> <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group input-group-flat"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control text-end pe-0"</span>  <span class="na">value=</span><span class="s">"yourfancydomain"</span> <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      .tabler.io
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;script&gt;</span>
  <span class="nx">noUiSlider</span><span class="p">.</span><span class="nx">create</span><span class="p">(</span><span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="dl">'</span><span class="s1">range-color</span><span class="dl">'</span><span class="p">),</span> <span class="p">{</span>
  	<span class="na">start</span><span class="p">:</span> <span class="mi">40</span><span class="p">,</span>
  	<span class="na">connect</span><span class="p">:</span> <span class="p">[</span><span class="kc">true</span><span class="p">,</span> <span class="kc">false</span><span class="p">],</span>
  	<span class="na">step</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
  	<span class="na">range</span><span class="p">:</span> <span class="p">{</span>
  		<span class="na">min</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
  		<span class="na">max</span><span class="p">:</span> <span class="mi">100</span>
  	<span class="p">}</span>
  <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="input-with-appended-link">Input with appended link</h2>
                      <p>Include a link in your input control to add a clickable element within the control.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Input with appended link</label>
                            <div class="input-group input-group-flat">
                              <input type="password" class="form-control" value="ultrastrongpassword" autocomplete="off">
                              <span class="input-group-text">
                                <a href="javascript:void(0)" class="input-group-link">Show password</a>
                              </span>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Input with appended link<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group input-group-flat"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"password"</span> <span class="na">class=</span><span class="s">"form-control"</span>  <span class="na">value=</span><span class="s">"ultrastrongpassword"</span> <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"#"</span> <span class="na">class=</span><span class="s">"input-group-link"</span><span class="nt">&gt;</span>Show password<span class="nt">&lt;/a&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;script&gt;</span>
  <span class="nx">noUiSlider</span><span class="p">.</span><span class="nx">create</span><span class="p">(</span><span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="dl">'</span><span class="s1">range-color</span><span class="dl">'</span><span class="p">),</span> <span class="p">{</span>
  	<span class="na">start</span><span class="p">:</span> <span class="mi">40</span><span class="p">,</span>
  	<span class="na">connect</span><span class="p">:</span> <span class="p">[</span><span class="kc">true</span><span class="p">,</span> <span class="kc">false</span><span class="p">],</span>
  	<span class="na">step</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
  	<span class="na">range</span><span class="p">:</span> <span class="p">{</span>
  		<span class="na">min</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
  		<span class="na">max</span><span class="p">:</span> <span class="mi">100</span>
  	<span class="p">}</span>
  <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span></code></pre>
                        </figure>
                      </div>
                      <h2 id="input-with-appended-icon-links">Input with appended icon links</h2>
                      <p>Add an icon link which you want to display at the end of your input control to visually represent actions which a user can take.</p>
                      <div class="example no_toc_section">
                        <div class="example-content">
                          <div class="mb-3">
                            <label class="form-label">Input with appended icon links</label>
                            <div class="input-group input-group-flat">
                              <input type="text" class="form-control" autocomplete="off">
                              <span class="input-group-text">
                                <a href="javascript:void(0)" class="link-secondary" title="" data-bs-toggle="tooltip" data-bs-original-title="Clear search"><!-- Download SVG icon from http://tabler-icons.io/i/x -->
                                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line></svg>
                                </a>
                                <a href="javascript:void(0)" class="link-secondary ms-2" title="" data-bs-toggle="tooltip" data-bs-original-title="Search settings"><!-- Download SVG icon from http://tabler-icons.io/i/adjustments -->
                                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><circle cx="6" cy="10" r="2"></circle><line x1="6" y1="4" x2="6" y2="8"></line><line x1="6" y1="12" x2="6" y2="20"></line><circle cx="12" cy="16" r="2"></circle><line x1="12" y1="4" x2="12" y2="14"></line><line x1="12" y1="18" x2="12" y2="20"></line><circle cx="18" cy="7" r="2"></circle><line x1="18" y1="4" x2="18" y2="5"></line><line x1="18" y1="9" x2="18" y2="20"></line></svg>
                                </a>
                                <a href="javascript:void(0)" class="link-secondary ms-2 disabled" title="" data-bs-toggle="tooltip" data-bs-original-title="Add notification"><!-- Download SVG icon from http://tabler-icons.io/i/bell -->
                                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><path d="M10 5a2 2 0 0 1 4 0a7 7 0 0 1 4 6v3a4 4 0 0 0 2 3h-16a4 4 0 0 0 2 -3v-3a7 7 0 0 1 4 -6"></path><path d="M9 17v1a3 3 0 0 0 6 0v-1"></path></svg>
                                </a>
                              </span>
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="example-code">
                        <figure class="highlight">
                          <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"mb-3"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;label</span> <span class="na">class=</span><span class="s">"form-label"</span><span class="nt">&gt;</span>Input with appended icon links<span class="nt">&lt;/label&gt;</span>
  <span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"input-group input-group-flat"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;input</span> <span class="na">type=</span><span class="s">"text"</span> <span class="na">class=</span><span class="s">"form-control"</span>  <span class="na">autocomplete=</span><span class="s">"off"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"input-group-text"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"#"</span> <span class="na">class=</span><span class="s">"link-secondary"</span> <span class="na">title=</span><span class="s">"Clear search"</span> <span class="na">data-bs-toggle=</span><span class="s">"tooltip"</span><span class="nt">&gt;</span><span class="c">&lt;!-- Download SVG icon from http://tabler-icons.io/i/x --&gt;</span>
        <span class="c">&lt;!-- SVG icon code --&gt;</span>
      <span class="nt">&lt;/a&gt;</span>
      <span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"#"</span> <span class="na">class=</span><span class="s">"link-secondary ms-2"</span> <span class="na">title=</span><span class="s">"Search settings"</span> <span class="na">data-bs-toggle=</span><span class="s">"tooltip"</span><span class="nt">&gt;</span><span class="c">&lt;!-- Download SVG icon from http://tabler-icons.io/i/adjustments --&gt;</span>
        <span class="c">&lt;!-- SVG icon code --&gt;</span>
      <span class="nt">&lt;/a&gt;</span>
      <span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"#"</span> <span class="na">class=</span><span class="s">"link-secondary ms-2 disabled"</span> <span class="na">title=</span><span class="s">"Add notification"</span> <span class="na">data-bs-toggle=</span><span class="s">"tooltip"</span><span class="nt">&gt;</span><span class="c">&lt;!-- Download SVG icon from http://tabler-icons.io/i/bell --&gt;</span>
        <span class="c">&lt;!-- SVG icon code --&gt;</span>
      <span class="nt">&lt;/a&gt;</span>
    <span class="nt">&lt;/span&gt;</span>
  <span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;script&gt;</span>
  <span class="nx">noUiSlider</span><span class="p">.</span><span class="nx">create</span><span class="p">(</span><span class="nb">document</span><span class="p">.</span><span class="nx">getElementById</span><span class="p">(</span><span class="dl">'</span><span class="s1">range-color</span><span class="dl">'</span><span class="p">),</span> <span class="p">{</span>
  	<span class="na">start</span><span class="p">:</span> <span class="mi">40</span><span class="p">,</span>
  	<span class="na">connect</span><span class="p">:</span> <span class="p">[</span><span class="kc">true</span><span class="p">,</span> <span class="kc">false</span><span class="p">],</span>
  	<span class="na">step</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
  	<span class="na">range</span><span class="p">:</span> <span class="p">{</span>
  		<span class="na">min</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
  		<span class="na">max</span><span class="p">:</span> <span class="mi">100</span>
  	<span class="p">}</span>
  <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span></code></pre>
                        </figure>
                      </div>
                    </div>