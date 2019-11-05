# read6
CHECKING EQUALITY
& EXISTENCE
Because the presence of an object or array can
be considered truthy, it is often used to check
for the existence of an element within a page.
A unary operator returns a
result with just one operand.
Here you can see an if
statement checking for the
presence of an element. If the
element is found, the result is
truthy, so the first set of code is
run. If it is not found, the second
set is run instead.
if (document .getElementByid('header'))
II Found: do something
else {
II Not found: do somethi ng else
Those new to JavaScript often think the following would do the same:
if (document .getElementByld('header') ==true)
but document.getEl ementByld ('header') would return an object
which is a truthy value but it is not equal to a Boolean value of true.
Because of type coercion, the strict equality operators ===and ! == result
in fewer unexpected values than ==and ! = do.
If you use == the following values
can be considered equal:
false, 0, and ' ' (empty string).
However, they are not equivalent
when using the strict operators.
EXPRESSION
(false == 0)
(false === 0)
RESULT
true
false
(false== ") true
(false === ' ') false
(0 :: I I)
(O === II)
8 DECISIONS & LOOPS
true
false
Although null and undefined are
both falsy, they are not equal to
anything other than themselves.
Again, they are not equivalent
when using strict operators.
EXPRESSION RESULT
(undefined ==null) true
(null == false) false
(undefi ned == false) fa l se
(null == 0) false
(undefined == O) false
(undefined === null) fals

getElementsByTagName('hl ' )
Even though this query only
returns one element. the method
still returns a Nodelist because
of the potential for returning
more than one element.
INDEX NUMBER & ELEMENT
0 <hl>
getElementsByTagName('li ')
This method returns four
elements, one for each of the
<l i> elements on the page.
They appear in the same order
as they do in the HTML page.
INDEX NUMBER & ELEMENT
0 <li i d•"one" class="hot">
1 <1 i i d="two" cl ass="hot">
2 <l i id="three" class• "hot">
3 <li id="four">
getElementsByClassName('hot')
This Nodelist contains only
three of the <l i >elements
because we are searching for
elements by the value of their
cl ass attribute, not tag name.
INDEX NUMBER & ELEMENT
O <li id="one" cl ass="hot">
l <li id=" two" class="hot">
2 <l i id=" three" class="hot">
querySe l ectorA 11 ( ' l i [id] ' )
This method returns four
elements, one for each of the
<l i> elements on the page that
have an id attribute (regardless
of the values of the id attributes).
INDEX NUMBER & ELEMENT
O <l i id="one" class="hot">
1 c ] j id="two" class="hot">
2 <li id=" three" class="hot">
3 <li id• "four"> 
