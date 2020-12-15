description: RNNCell wrapper that ensures cell inputs are added to the outputs.

<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="tf.compat.v1.nn.rnn_cell.ResidualWrapper" />
<meta itemprop="path" content="Stable" />
<meta itemprop="property" content="__init__"/>
<meta itemprop="property" content="__new__"/>
<meta itemprop="property" content="get_initial_state"/>
<meta itemprop="property" content="zero_state"/>
</div>

# tf.compat.v1.nn.rnn_cell.ResidualWrapper

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent" align="left">
<td>
  <a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r2.3/tensorflow/python/keras/layers/legacy_rnn/rnn_cell_impl.py#L1185-L1192">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td>
</table>



RNNCell wrapper that ensures cell inputs are added to the outputs.

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>tf.compat.v1.nn.rnn_cell.ResidualWrapper(
    *args, **kwargs
)
</code></pre>



<!-- Placeholder for "Used in" -->


<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Args</h2></th></tr>

<tr>
<td>
`cell`
</td>
<td>
An instance of `RNNCell`.
</td>
</tr><tr>
<td>
`residual_fn`
</td>
<td>
(Optional) The function to map raw cell inputs and raw cell
outputs to the actual cell outputs of the residual network.
Defaults to calling nest.map_structure on (lambda i, o: i + o), inputs
and outputs.
</td>
</tr><tr>
<td>
`**kwargs`
</td>
<td>
dict of keyword arguments for base layer.
</td>
</tr>
</table>





<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Attributes</h2></th></tr>

<tr>
<td>
`graph`
</td>
<td>
DEPRECATED FUNCTION

Warning: THIS FUNCTION IS DEPRECATED. It will be removed in a future version.
Instructions for updating:
Stop using this property because tf.layers layers no longer track their graph.
</td>
</tr><tr>
<td>
`output_size`
</td>
<td>

</td>
</tr><tr>
<td>
`scope_name`
</td>
<td>

</td>
</tr><tr>
<td>
`state_size`
</td>
<td>

</td>
</tr>
</table>



## Methods

<h3 id="get_initial_state"><code>get_initial_state</code></h3>

<a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r2.3/tensorflow/python/keras/layers/legacy_rnn/rnn_cell_impl.py#L281-L309">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>get_initial_state(
    inputs=None, batch_size=None, dtype=None
)
</code></pre>




<h3 id="zero_state"><code>zero_state</code></h3>

<a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r2.3/tensorflow/python/keras/layers/legacy_rnn/rnn_cell_wrapper_impl.py#L348-L350">View source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>zero_state(
    batch_size, dtype
)
</code></pre>





