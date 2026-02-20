 - Дерево обхода DFS - 
 - Мост - 

___

#### Алгоритм находения мостов

```python
dfs(v, p): # p - вершина, из которой пришли в v
	tin[v] = timer++ # время входа
	used[v] = true
	up[v] = tin[v] # 
	for (u : graph[v])::
		if (u == p) continue
		if (!used[u]):
			dfs(u, v)
			up[v] = min(up[v], up[u])
			
			if (tin[v] < up[u])
				# (v, u) - мост
		else:
			up[v] = min(up[v], tin[u])
```

*+ итеративный подход через buf*

___

- Точка сочленения - 

#### Алгоритм находения точек сочленения

___

### Кратчайшее расстояние

### $w_{u,v} = 1$

```cpp
dist = {-1, -1, ...}
dist[start] = 0
queue.push(start)

while (!queue.empty()) {
	v = queue.front()
	queue.pop()
	
	for (u : graph[v]) {
		if (dist[u] == -1) {
			dist[u] = dist[v] + 1
			q.push(u)
		}
	}
}
```

___

#### $w_{u, v} \in \{ 1, \dots, k \}$

___
#### $w_{u, v} > 0$

___

#### $w_{u, v} \in \mathbb{R}$



