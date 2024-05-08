<template>
  <h2>Button with Tailwind CSS</h2>
  <button class="px-6 py-4 rounded-md bg-indigo-600 text-xl font-semibold text-white shadow-sm hover:bg-indigo-500">
    Example Button
  </button>
  <blockquote>
    A well-padded, moderately rounded indigo button with large, semi-bold white text. It has a small shadow, and its color becomes lighter when it is hovered over.
  </blockquote>
  <pre><code>&lt;button class=&quot;px-6 py-4 rounded-md bg-indigo-600 text-xl font-semibold text-white shadow-sm hover:bg-indigo-500&quot;&gt;
  Example Button
&lt;/button&gt;</code></pre>
<details>
<summary>Break it down...</summary>
<ul>
  <li><code>rounded-md</code>: Set the border-radius property to 0.375rem</li>
  <li><code>bg-indigo-600</code>: Apply background-color property with a hexadecimal value of a dark shade of indigo.</li>
  <li><code>px-6</code>: Apply padding-left and padding-right properties equivalent to 1.5rem, providing space around <em>horizontally</em>.</li>
  <li><code>py-4</code>: Apply padding-top and padding-bottom properties equivalent to 1rem, providing space around <em>vertically</em>.</li>
  <li><code>text-xl</code>: Set the font-size property to 1.25rem, and line-height to 1.75rem.</li>
  <li><code>font-semibold</code>: Set font-weight property to 600.</li>
  <li><code>text-white</code>: Apply a color property with the value of white.</li>
  <li><code>shadow-sm</code>: Apply a box-shadow property.</li>
  <li><code>hover:bg-indigo-500</code>: With a hover state pseudo-class, apply a background-color property with a different hexadecimal value for a lighter shade of indigo.</li>
</ul>

</details>
</template>
