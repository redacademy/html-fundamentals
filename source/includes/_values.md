##Passing by Value vs. Passing by Reference

#Passing by Reference
You're in an university class, given a topic on __Passing by Reference__. Your
whole class is really struggling with the paper and everyone is complaining,
wanting a topic change. But unfortunately, Professor JavaScript sees the value
in the topic and it will never change. So consider this, even though the
topic, or value, never changes, the papers handed in can have different
contents but the topic never changes. In essence, now when talking about
__Passing by Reference__ all those papers can be handed in no matter the
attributes of those papers.

```js
var paperTopic = [paper1, paper2, paper3, paper4];

Values in the array can be changed,
but the topic, or value of the array,
never changes.
```

#Passing by Value

Conversely, Professor JavaScript doesn't like you. He makes you handwrite
your paper, but also, for some ridiculous reason, wants you to hand in a
photocopy. After handing it in you frame your handwritten paper, so it never
changes. Meanwhile, Professor JavaScript figuratively shits on your paper, changing
it forever, but he shall never touch your handwritten 'masterpiece'.

```js
var handwritten = yourHandwrittenPaper

(fn (changePaper) {
  return handwritten + '49%'
}
'yourHandwrittenPaper 49%'
)

Handwritten can be called and changed
in a function, but the original
value of the handwritten variable
never changes
```

#Pure function

__Pure function__ is a pipe that doesn't leak, and in essence cannot be mutated.
Some of the benefits of using a pure function clarity,
cleanliness, the job is done more percisely. Moreover, it will not unintentionally
effect scripts running in other parts of your code.