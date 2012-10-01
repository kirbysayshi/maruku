C-like syntax within a `<code>` tag should not bork.
*** Parameters: ***
{}
*** Markdown input: ***
<figure>
    <a id="fig-14"></a>
    <pre><code>
hashA = entityA._roId + ':' + entityB._roId;
hashB = entityB._roId + ':' + entityA._roId;

if( !checked[hashA] && !checked[hashB] ){

    // mark this pair as checked
    checked[hashA] = checked[hashB] = true;

    if( this.aabb2DIntersection( entityA, entityB ) ){
        pairs.push( [entityA, entityB] );
    }
}
    </code></pre>
    <figcaption>
        Fig. 14: Keeping a cache of tested pairs.
    </figcaption>
</figure>
*** Output of inspect ***
md_el(:document,[
	md_html("<figure>\n    <a id=\"fig-14\"></a>\n    <pre><code>\nhashA = entityA._roId + ':' + entityB._roId;\nhashB = entityB._roId + ':' + entityA._roId;\n\nif( !checked[hashA] && !checked[hashB] ){\n\n    // mark this pair as checked\n    checked[hashA] = checked[hashB] = true;\n\n    if( this.aabb2DIntersection( entityA, entityB ) ){\n        pairs.push( [entityA, entityB] );\n    }\n}\n    </code></pre>\n    <figcaption>\n        Fig. 14: Keeping a cache of tested pairs.\n    </figcaption>\n</figure>")
],{},[])
*** Output of to_html ***
<figure>
    <a id="fig-14"></a>
    <pre><code>
hashA = entityA._roId + ':' + entityB._roId;
hashB = entityB._roId + ':' + entityA._roId;

if( !checked[hashA] && !checked[hashB] ){

    // mark this pair as checked
    checked[hashA] = checked[hashB] = true;

    if( this.aabb2DIntersection( entityA, entityB ) ){
        pairs.push( [entityA, entityB] );
    }
}
    </code></pre>
    <figcaption>
        Fig. 14: Keeping a cache of tested pairs.
    </figcaption>
</figure>
*** Output of to_latex ***
 Fig. 14: Keeping a cache of tested pairs.
*** Output of to_md ***
<figure>
    <a id="fig-14"></a>
    <pre><code>
hashA = entityA._roId + ':' + entityB._roId;
hashB = entityB._roId + ':' + entityA._roId;

if( !checked[hashA] && !checked[hashB] ){

    // mark this pair as checked
    checked[hashA] = checked[hashB] = true;

    if( this.aabb2DIntersection( entityA, entityB ) ){
        pairs.push( [entityA, entityB] );
    }
}
    </code></pre>
    <figcaption>
        Fig. 14: Keeping a cache of tested pairs.
    </figcaption>
</figure>
*** Output of to_s ***

