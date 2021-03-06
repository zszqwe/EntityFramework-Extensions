---
permalink: batch
---

### BatchSize
Gets or sets the number of records to use in a batch.

{% include template-example.html %} 
{% highlight csharp %}
context.BulkSaveChanges(options => options.BatchSize = 1000);
{% endhighlight %}
{% include component-try-it.html href='https://dotnetfiddle.net/BThvHs' %}

---

### BatchTimeout
Gets or sets the maximum in seconds to wait for a batch before the command throws a timeout exception.

{% include template-example.html %} 
{% highlight csharp %}
context.BulkSaveChanges(options => options.BatchTimeout = 180);
{% endhighlight %}
{% include component-try-it.html href='https://dotnetfiddle.net/HDmeWa' %}

---

### BatchDelayInterval
Gets or sets a delay in milliseconds to wait between batches.

{% include template-example.html %} 
{% highlight csharp %}
context.BulkInsert(list, options => options.BatchDelayInterval = 100);
{% endhighlight %}
{% include component-try-it.html href='https://dotnetfiddle.net/65v3k3' %}
