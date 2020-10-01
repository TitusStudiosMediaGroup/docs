# Hello World!

{% highlight livescript linenos %}
@name Cool E2 Name
@inputs MyInput MyInput2
@outputs MyOutput MyOutput2 MyOutput3
@persist [E]:entity MyVar [Color]:vector
@trigger none
@model models/jazzie/trains/locomotives/emd/cab/battery_panel_gp28-35.mdl

function void isolateSubMaterial(TargetHolo,IsolationArray:array,KeepSub,TotalSubMaterials,IsolatedMaterialOverride:string) {
    local InvisibleTexture = "models/proppertextures/invisible"

    # Comment time!

    #[
        Comment Blocks work too!
        Wowie.
    ]#

    for (N=1,IsolationArray:count()) {
        holoEntity(IsolationArray[N,number]):setSubMaterial(KeepSub,InvisibleTexture)
    }

    for (N=1,TotalSubMaterials) {
        holoEntity(TargetHolo):setSubMaterial(N,InvisibleTexture)
    }

    holoEntity(TargetHolo):setSubMaterial(KeepSub,IsolatedMaterialOverride)
} 
{% endhighlight %}
