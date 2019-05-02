#### 1. animate()
CSS position attribute: relative, fixed or absolute

#### 2. Callback
Make sure callback function runs after updating UI

#### 3. Chaining
* Don't need to find element everytime
* Indentation is important

#### 4. DOM
* ##### Get
    * text(): text
    * html(): text and tag
    * val(): input value
    * attr(): element attribute
* ##### Set
    * text(text): text
    * html(html): text and tag
    * val(value): input value
    * attr(attr): element attribute
    * attr({attr1, attr2...}): element attribute
    * text(function(i,origText)): text
    * html(function(i,origText)): text and tag
    * val(function(i,origText)): input value
    * attr(function(i,origValue)): element attribute
* ##### Add
    * append(text1, text2...)/prepend(text1, text2...): content
    * before(text1, text2...)/after(text1, text2...): position
* ##### Delete
    * remove()
    * remove(filter): ".class"
    * empty()
* ##### CSS
    * addClass("class1 class2 ...")
    * removeClass("class")
    * toggleClass("class")
    * css({"propertyname":"value","propertyname":"value",...});

#### 5. Size
* width()/height(): without padding, border, margin
* innerWidth()/innerHeight(): without border, margin
* outerWidth()/outerHeight(): without margin

#### 6. Retrival DOM Tree
* ##### Parents/Children
    * parent()/children()
    * parents(filter, filter...)/find(*)
    * parentUntil(filter)/find(filter)
* ##### Siblings
    * siblings()
    * next()
    * nextAll()
    * nextUntil()
    * prev()
    * prevAll()
    * prevUntil()
* ##### Index
    * first()
    * last()
    * eq(order): order starts from 0

#### 7. AJAX
* Load: $(selector).load(URL,data,function(responseTxt,statusTxt,xhr)): data-namevaluepair, xhr-XMLHttpRequest(data object)
* Get: $.get(URL,function(data,status));
* Post: $.post(URL,data,function(data,status));

#### 8. '$' conflict
* $.noConflict();->jQuery
* var jq = $.noConflict();->jq

