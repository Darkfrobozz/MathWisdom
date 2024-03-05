
Any vector can be formed by addition and scaling of the [[basis_vectors]]. Thus, we can represent any area representable by scaling and adding to those [[basis_vectors]].
### Scaling
When scaling we simply apply the scalar to the area, this makes sense because of symmetry, we can simply split up or take multiple of the original parallelogram and align them to get a new parallelogram with the decided scalar applied to the vector.
$$
\frac{1}{2}A = \left( \frac{1}{2}v, w  \right)
$$
### Addition
We can use the fact that vectors are [[commutative]] to realize that when we suppose that we have an area formed by:
$$
A(v, w)
$$
And then we add $u$ to $v$, we get that there are two triangles one formed by the vectors $v, u, v + u$ starting at 0 and one shifted up by $w$
![[Pasted image 20240304153645.png]]
The former is present in:
$$
A(v + u, w)
$$
while the latter is present in
$$
A(v,w) + A(u, w)
$$
This results in the very useful [[distrubitive]] result that:
$$
A(v+u, w) = A(v, w) + A(u,w)
$$
### Signed scaling
The sign of an area is often reduced to nonsense but there is an important property that it represents, namely orientation.
For example, the area is unsigned if v to w is a clockwise motion. And counter clockwise means a signed area.