C-like syntax within a `<code>` tag should not bork.
*** Parameters: ***
{}
*** Markdown input: ***
<figure>
	<a id="fig-2"></a>
	<pre><code>
BruteForceTech.prototype.queryForCollisionPairs = function(){

	var i, j, e1, e2, pairs = [], entityLen = this.entities.length;

	this.collisionTests = 0;

	for( i = 0; i < entityLen; i++ ){
		e1 = this.entities[i];

		for( j = i+1; j < entityLen; j++ ){
			e2 = this.entities[j];

			this.collisionTests += 1;

			if( this.aabb2DIntersection(e1, e2) === true ){
				pairs.push( [e1, e2] );
			}
		}
	}

	return pairs;
}

BruteForceTech.prototype.aabb2DIntersection = function( objA, objB ){
	var  a = objA.getAABB()
		,b = objB.getAABB();

	if(
		a.min[0] > b.max[0] || a.min[1] > b.max[1]
		|| a.max[0] < b.min[0] || a.max[1] < b.min[1]
	){
		return false;
	} else {
		return true;
	}
}
	</code></pre>
	<figcaption>
		Fig. 2: Two functions demonstrating brute force collision detection iteration and an AABB overlap test.
	</figcaption>
</figure>
*** Output of inspect ***
md_el(:document,[
	md_html("<figure>\n\t<a id=\"fig-2\"></a>\n\t<pre><code>\nBruteForceTech.prototype.queryForCollisionPairs = function(){\n\n\tvar i, j, e1, e2, pairs = [], entityLen = this.entities.length;\n\n\tthis.collisionTests = 0;\n\n\tfor( i = 0; i < entityLen; i++ ){\n\t\te1 = this.entities[i];\n\n\t\tfor( j = i+1; j < entityLen; j++ ){\n\t\t\te2 = this.entities[j];\n\n\t\t\tthis.collisionTests += 1;\n\n\t\t\tif( this.aabb2DIntersection(e1, e2) === true ){\n\t\t\t\tpairs.push( [e1, e2] );\n\t\t\t}\n\t\t}\n\t}\n\n\treturn pairs;\n}\n\nBruteForceTech.prototype.aabb2DIntersection = function( objA, objB ){\n\tvar  a = objA.getAABB()\n\t\t,b = objB.getAABB();\n\n\tif(\n\t\ta.min[0] > b.max[0] || a.min[1] > b.max[1]\n\t\t|| a.max[0] < b.min[0] || a.max[1] < b.min[1]\n\t){\n\t\treturn false;\n\t} else {\n\t\treturn true;\n\t}\n}\n\t</code></pre>\n\t<figcaption>\n\t\tFig. 2: Two functions demonstrating brute force collision detection iteration and an AABB overlap test.\n\t</figcaption>\n</figure>")
],{},[])
*** Output of to_html ***
<figure>
	<a id="fig-2"></a>
	<pre><code>
BruteForceTech.prototype.queryForCollisionPairs = function(){

	var i, j, e1, e2, pairs = [], entityLen = this.entities.length;

	this.collisionTests = 0;

	for( i = 0; i < entityLen; i++ ){
		e1 = this.entities[i];

		for( j = i+1; j < entityLen; j++ ){
			e2 = this.entities[j];

			this.collisionTests += 1;

			if( this.aabb2DIntersection(e1, e2) === true ){
				pairs.push( [e1, e2] );
			}
		}
	}

	return pairs;
}

BruteForceTech.prototype.aabb2DIntersection = function( objA, objB ){
	var  a = objA.getAABB()
		,b = objB.getAABB();

	if(
		a.min[0] > b.max[0] || a.min[1] > b.max[1]
		|| a.max[0] < b.min[0] || a.max[1] < b.min[1]
	){
		return false;
	} else {
		return true;
	}
}
	</code></pre>
	<figcaption>
		Fig. 2: Two functions demonstrating brute force collision detection iteration and an AABB overlap test.
	</figcaption>
</figure>
*** Output of to_latex ***
 Fig. 2: Two functions demonstrating brute force collision detection
iteration and an AABB overlap test.
*** Output of to_md ***
<figure>
	<a id="fig-2"></a>
	<pre><code>
BruteForceTech.prototype.queryForCollisionPairs = function(){

	var i, j, e1, e2, pairs = [], entityLen = this.entities.length;

	this.collisionTests = 0;

	for( i = 0; i < entityLen; i++ ){
		e1 = this.entities[i];

		for( j = i+1; j < entityLen; j++ ){
			e2 = this.entities[j];

			this.collisionTests += 1;

			if( this.aabb2DIntersection(e1, e2) === true ){
				pairs.push( [e1, e2] );
			}
		}
	}

	return pairs;
}

BruteForceTech.prototype.aabb2DIntersection = function( objA, objB ){
	var  a = objA.getAABB()
		,b = objB.getAABB();

	if(
		a.min[0] > b.max[0] || a.min[1] > b.max[1]
		|| a.max[0] < b.min[0] || a.max[1] < b.min[1]
	){
		return false;
	} else {
		return true;
	}
}
	</code></pre>
	<figcaption>
		Fig. 2: Two functions demonstrating brute force collision detection iteration and an AABB overlap test.
	</figcaption>
</figure>
*** Output of to_s ***

