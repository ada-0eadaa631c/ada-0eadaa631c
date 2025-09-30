# exercise1
1. variable name: .isidentifier()
* CamelCase-style: initial_velocity
* snake_case-style: InitialVelocity
2. 
* pybryt: automated assessment scoring
* assert: additional testing in case your solution is not covered with PyBryt references
3. Formatted printing style
* f-string: print(f"At t={t:g} s, y is {y:.2f} m.")  
g: expresses the floating-point number with the minimum number of significant figures  
.2f: only two digits are printed out after the decimal point
* `format` method: print("At t={:g} s, y is {:.2f} m.".format(t, y))
* `%` operator: print("At t=%g s, y is %.2f m." % (t, y))
4. ** power
5. math.sqrt, pi, sin, cos, log
6. No return value implies that `None` is returned. `None` is a special Python object (singleton) that semantically often represents an ”empty” or undefined value.
7. zip(list1, list2, ...)  
for e1, e2, e3 in zip(l1, l2, l3):   print(f"{e1 = }, {e2 = }, {e3 = }")
8. Tuples are actually not always immutable. If a tuple contains mutable elements, e.g. `list`, it is possible to change the tuple  
hash(t): check if the tuple is actually mutable
9. x2 = np.linspace(0, 1, n)    # generates n points between 0 and 1  
We can select a slice of an array using `a[start:stop:inc]`, where the slice `start:stop:inc` implies a set of indices starting from `start`, up to `stop` in increments `inc`. Any integer list or array can be used to indicate a set of indices  
np.linspace(1, 30, 30).reshape(5, 6)
10. .copy(): explicit copy
11. np.ndenumerate
12. NumPy provides a convenience operator `@` that can be applied between arrays of compatible shapes for multiplication
13. res = np.zeros([A.shape[0], B.shape[1]])
    for i in range(A.shape[0]):          # 遍历 A 的行
        for j in range(B.shape[1]):      # 遍历 B 的列
            for k in range(A.shape[1]):  # 遍历 A 的列 / B 的行
                res[i, j] += A[i, k] * B[k, j]
14. 