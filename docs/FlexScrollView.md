<a name="module_FlexScrollView"></a>
#FlexScrollView
Flexible FlexScrollView for famo.us.

Key features:
-    Customizable layout (uses ListLayout by default)
-    Insert/remove at any position using animations
-    Support for `true` size renderables
-    Pull to refresh (header & footer)
-    Horizontal/vertical direction
-    Top/left or bottom/right alignment
-    Pagination
-    Option to embed in a ContainerSurface
-    FlexScrollView linking

Inherited from: [ScrollController](./ScrollController.md)

<a name="exp_module_FlexScrollView"></a>
##class: FlexScrollView ⏏
**Extends**: `ScrollController`  
**Members**

* [class: FlexScrollView ⏏](#exp_module_FlexScrollView)
  * [new FlexScrollView(options)](#exp_new_module_FlexScrollView)
  * [~~flexScrollView.getPosition~~](#module_FlexScrollView#getPosition)
  * [flexScrollView.setOptions(options)](#module_FlexScrollView#setOptions)
  * [flexScrollView.sequenceFrom(node)](#module_FlexScrollView#sequenceFrom)
  * [flexScrollView.getCurrentIndex()](#module_FlexScrollView#getCurrentIndex)
  * [flexScrollView.goToPage(index)](#module_FlexScrollView#goToPage)
  * [flexScrollView.getOffset()](#module_FlexScrollView#getOffset)
  * [flexScrollView.showPullToRefresh([footer])](#module_FlexScrollView#showPullToRefresh)
  * [flexScrollView.hidePullToRefresh([footer])](#module_FlexScrollView#hidePullToRefresh)
  * [flexScrollView.isPullToRefreshVisible([footer])](#module_FlexScrollView#isPullToRefreshVisible)

<a name="exp_new_module_FlexScrollView"></a>
###new FlexScrollView(options)
**Params**

- options `Object` - Configurable options (see ScrollController for all inherited options).  
  - \[pullToRefreshHeader\] `Renderable` - Pull to refresh renderable that is displayed when pulling down from the top.  
  - \[pullToRefreshFooter\] `Renderable` - Pull to refresh renderable that is displayed when pulling up from the bottom.  
  - \[leadingScrollView\] `FlexScrollView` - Leading scrollview into which input events are piped (see Tutorial)  
  - \[trailingScrollView\] `FlexScrollView` - Trailing scrollview into which input events are piped (see Tutorial)  

**Extends**: `ScrollController`  
<a name="module_FlexScrollView#getPosition"></a>
###~~flexScrollView.getPosition~~
Returns the position associated with the Scrollview instance's current node
(generally the node currently at the top).

This function is a shim provided for compatibility with the stock famo.us Scrollview.

**Params**

- \[node\] `number` - If specified, returns the position of the node at that index in the
Scrollview instance's currently managed collection.  

***Deprecated***  
**Returns**: `number` - The position of either the specified node, or the Scrollview's current Node,
in pixels translated.  
<a name="module_FlexScrollView#setOptions"></a>
###flexScrollView.setOptions(options)
Patches the FlexScrollView instance's options with the passed-in ones.

**Params**

- options `Object` - Configurable options (see ScrollController for all inherited options).  
  - \[pullToRefreshHeader\] `Renderable` - Pull to refresh renderable that is displayed when pulling down from the top.  
  - \[pullToRefreshFooter\] `Renderable` - Pull to refresh renderable that is displayed when pulling up from the bottom.  
  - \[leadingScrollView\] `FlexScrollView` - Leading scrollview into which input events are piped (see Tutorial).  
  - \[trailingScrollView\] `FlexScrollView` - Trailing scrollview into which input events are piped (see Tutorial).  

**Returns**: `FlexScrollView` - this  
<a name="module_FlexScrollView#sequenceFrom"></a>
###flexScrollView.sequenceFrom(node)
Sets the data-source (alias for setDataSource).

This function is a shim provided for compatibility with the stock famo.us Scrollview.

**Params**

- node `Array` | `ViewSequence` - Either an array of renderables or a Famous viewSequence.  

**Returns**: `FlexScrollView` - this  
<a name="module_FlexScrollView#getCurrentIndex"></a>
###flexScrollView.getCurrentIndex()
Returns the index of the first visible renderable.

This function is a shim provided for compatibility with the stock famo.us Scrollview.

**Returns**: `Number` - The current index of the ViewSequence  
<a name="module_FlexScrollView#goToPage"></a>
###flexScrollView.goToPage(index)
Paginates the Scrollview to an absolute page index. This function is a shim provided
for compatibility with the stock famo.us Scrollview.

**Params**

- index `Number` - view-sequence index to go to.  

**Returns**: `FlexScrollView` - this  
<a name="module_FlexScrollView#getOffset"></a>
###flexScrollView.getOffset()
Returns the offset associated with the Scrollview instance's current node
(generally the node currently at the top).

This function is a shim provided for compatibility with the stock famo.us Scrollview.

**Returns**: `number` - The position of either the specified node, or the Scrollview's current Node,
in pixels translated.  
<a name="module_FlexScrollView#showPullToRefresh"></a>
###flexScrollView.showPullToRefresh([footer])
Shows the pulls-to-refresh renderable indicating that a refresh is in progress.

**Params**

- \[footer\] `Bool` - set to true to show pull-to-refresh at the footer (default: false).  

**Returns**: `FlexScrollView` - this  
<a name="module_FlexScrollView#hidePullToRefresh"></a>
###flexScrollView.hidePullToRefresh([footer])
Hides the pull-to-refresh renderable in case it was visible.

**Params**

- \[footer\] `Bool` - set to true to hide the pull-to-refresh at the footer (default: false).  

**Returns**: `FlexScrollView` - this  
<a name="module_FlexScrollView#isPullToRefreshVisible"></a>
###flexScrollView.isPullToRefreshVisible([footer])
Get the visible state of the pull-to-refresh renderable.

**Params**

- \[footer\] `Bool` - set to true to get the state of the pull-to-refresh footer (default: false).  

