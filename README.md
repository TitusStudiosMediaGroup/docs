# Hello World!

{% highlight livescript linenos %}
function void isolateSubMaterial(TargetHolo,IsolationArray:array,KeepSub,TotalSubMaterials,IsolatedMaterialOverride:string) {
    local InvisibleTexture = "models/proppertextures/invisible"

    for (N=1,IsolationArray:count()) {
        holoEntity(IsolationArray[N,number]):setSubMaterial(KeepSub,InvisibleTexture)
    }

    for (N=1,TotalSubMaterials) {
        holoEntity(TargetHolo):setSubMaterial(N,InvisibleTexture)
    }

    holoEntity(TargetHolo):setSubMaterial(KeepSub,IsolatedMaterialOverride)
} 
{% endhighlight %}
