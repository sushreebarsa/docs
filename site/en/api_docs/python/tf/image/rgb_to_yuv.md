description: Converts one or more images from RGB to YUV.

<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="tf.image.rgb_to_yuv" />
<meta itemprop="path" content="Stable" />
</div>

# tf.image.rgb_to_yuv

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">
<td>
  <a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r2.3/tensorflow/python/ops/image_ops_impl.py#L3252-L3272">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td>
</table>



Converts one or more images from RGB to YUV.

<section class="expandable">
  <h4 class="showalways">View aliases</h4>
  <p>
<b>Compat aliases for migration</b>
<p>See
<a href="https://www.tensorflow.org/guide/migrate">Migration guide</a> for
more details.</p>
<p>`tf.compat.v1.image.rgb_to_yuv`</p>
</p>
</section>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>tf.image.rgb_to_yuv(
    images
)
</code></pre>



<!-- Placeholder for "Used in" -->

Outputs a tensor of the same shape as the `images` tensor, containing the YUV
value of the pixels.
The output is only well defined if the value in images are in [0,1].

<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Args</h2></th></tr>

<tr>
<td>
`images`
</td>
<td>
2-D or higher rank. Image data to convert. Last dimension must be
size 3.
</td>
</tr>
</table>



<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Returns</h2></th></tr>

<tr>
<td>
`images`
</td>
<td>
tensor with the same shape as `images`.
</td>
</tr>
</table>
