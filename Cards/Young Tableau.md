---
tags:
  - Area/Math/Combinatorics
  - Area/Math/Algebra/Group/PermutationGroup
  - Area/Math/Representation
---
**Young tableaux** are [[Cards/Young Diagram|Young diagrams]] filled with positive natural numbers with extra conditions.

A **semistandard Young tableau** $T$ of shape $[\lambda]=\{ \lambda_{1},\cdots,\lambda_{n} \}$ (a [[Partition|partition]]) is an indexed set of positive natural numbers $\{ T_{ij}:1\leq i\leq n,j=j(i)\in[1,\lambda_{i}] \}$ such that these labels are
1.  weakly increasing along the rows: $\forall i,j_{1}>j_{2}\to T_{ij_{1}}\geq T_{ij_{2}}$.
2. strictly increasing along the columns: $\forall j,i_{1}>i_{2}\to T_{i_{1}j}>T_{i_{2}j}$.

A **standard Young tableau** is a semistandard Young tableau with no repeated label.

For example, the shape $[2,1]$ has following semistandard Young tableaux:
<div class="young-wrap">
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">1</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">2</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">1</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">3</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">2</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">2</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">2</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">3</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">3</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">2</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">3</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">3</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">2</div>
		    <div class="young-cell">2</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">3</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">2</div>
		    <div class="young-cell">3</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">3</div>
	    </div>
	</div>
</div>

and following standard Young tableaux
<div class="young-wrap">
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">2</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">3</div>
	    </div>
	</div>
	<div class="young-tableau">
		<div class="young-row">
		    <div class="young-cell">1</div>
		    <div class="young-cell">3</div>
	    </div>
	    <div class="young-row">
		    <div class="young-cell">2</div>
	    </div>
	</div>
</div>
