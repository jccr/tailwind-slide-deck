<style scoped>
.btn-primary {
  zoom: 1.5;
  border-radius: 0.375rem;
  background-color: #4f46e5;
  padding: 0.5rem 0.75rem;
  font-size: 0.875rem;
  line-height: 1.25rem;
  font-weight: 600;
  color: #fff;
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
}

.btn-primary:hover {
  background-color: #6366f1;
}

.btn-primary:focus-visible {
  outline: 2px solid #4c6ef5;
  outline-offset: 2px;
}

.media-card {
  background-color: white;
  border: 1px solid hsl(0, 0%, 85%);
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}
.media-card__image {
  display: block;
  width: 100%;
  height: auto;
}
.media-card__content {
  padding: 1rem;
}
.media-card__title {
  font-size: 1.25rem;
  color: rgba(0, 0, 0, 0.8);
}
.media-card__body {
  font-size: 1rem;
  color: rgba(0, 0, 0, 0.75);
  line-height: 1.5;
}
</style>

<template>
  <h1>How do you use it?</h1>
  <h3>Step 1</h3>
  <details>
    <summary>Forget about writing CSS</summary>
    <div class="flex items-center gap-8">
      <div>
        <button class="btn-primary">Example Button</button>
      </div>
      <pre>&lt;button class=&quot;btn-primary&quot;&gt;Example Button&lt;/button&gt;</pre>
    </div>
    
    <pre>
.btn-primary {
  border-radius: 0.375rem;
  background-color: #4f46e5;
  padding: 0.5rem 0.75rem;
  font-size: 0.875rem;
  line-height: 1.25rem;
  font-weight: 600;
  color: #fff;
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
}

.btn-primary:hover {
  background-color: #6366f1;
}

.btn-primary:focus-visible {
  outline: 2px solid #4C6EF5;
  outline-offset: 2px;
}
</pre
    >
  </details>

  <details>
    <!-- <button type="button" class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Button text</button> -->
    <summary>Forget about naming classes, selectors, BEM...</summary>
    <div class="grid gap-2">
      <div class="w-64 p-4">
        <div class="media-card sticky top-4">
          <img
            class="media-card__image"
            src="https://cdn-images-1.medium.com/max/1600/0*o3c1g40EXj65Fq9k."
            alt=""
          />
          <div class="media-card__content">
            <h2 class="media-card__title">Adam Wathan</h2>
            <p class="media-card__body">
              Adam is a rad dude who likes TDD, Active Record, and garlic bread
              with cheese. He also hosts a decent podcast and has never had a
              really great haircut.
            </p>
          </div>
        </div>
      </div>
      <div class="col-start-2 grid-rows-2">
        <p>
          HTML
          <pre><code>&lt;div class=&quot;media-card&quot;&gt;
  &lt;img class=&quot;media-card__image&quot; src=&quot;https://cdn-images-1.medium.com/max/1600/0*o3c1g40EXj65Fq9k.&quot; alt=&quot;&quot;&gt;
  &lt;div class=&quot;media-card__content&quot;&gt;
    &lt;h2 class=&quot;media-card__title&quot;&gt;Adam Wathan&lt;/h2&gt;
    &lt;p class=&quot;media-card__body&quot;&gt;
      Adam is a rad dude who likes TDD, Active Record, and garlic bread with cheese. He also hosts a decent podcast and has never had a really great haircut.
    &lt;/p&gt;
  &lt;/div&gt;
&lt;/div&gt;
</code></pre>
        </p>
        <p>
          CSS
          <pre>
.media-card {
  background-color: white;
  border: 1px solid hsl(0, 0%, 85%);
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}
.media-card__image {
  display: block;
  width: 100%;
  height: auto;
}
.media-card__content {
  padding: 1rem;
}
.media-card__title {
  font-size: 1.25rem;
  color: rgba(0, 0, 0, 0.8);
}
.media-card__body {
  font-size: 1rem;
  color: rgba(0, 0, 0, 0.75);
  line-height: 1.5;
}
      </pre>
        </p>
      </div>
    </div>
  </details>
</template>
