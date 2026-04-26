#include <stdio.h>

#define V 5

void findVertexCover(int graph[V][V]) {
    int visited[V] = {0};

    for (int u = 0; u < V; u++) {
        if (!visited[u]) {
            for (int v = 0; v < V; v++) {
                if (graph[u][v] && !visited[v]) {
                    visited[u] = 1;
                    visited[v] = 1;
                    break;
                }
            }
        }
    }

    printf("Approximate Vertex Cover:\n");
    for (int i = 0; i < V; i++) {
        if (visited[i])
            printf("%d ", i);
    }
}

int main() {
    int graph[V][V] = {
        {0,1,0,0,0},
        {1,0,1,1,0},
        {0,1,0,1,1},
        {0,1,1,0,1},
        {0,0,1,1,0}
    };

    findVertexCover(graph);
    return 0;
}
