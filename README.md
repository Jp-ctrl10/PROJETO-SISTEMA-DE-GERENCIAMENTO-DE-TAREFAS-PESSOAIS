# PROJETO-SISTEMA-DE-GERENCIAMENTO-DE-TAREFAS-PESSOAIS
5 etapas e etapa final
/////////////////////////////////////////////////////////


etapa o4 #include <stdio.h>
#define maxTarefas 3 

struct Tarefa{
    int id;
    char descricao[50];
    int prioridade;
};
int main(){ 
    struct Tarefa listaDeTarefas[maxTarefas] = {
        { 1, "Comprar Pao", 1 },
        { 2, "Ir a Academia", 2 },
        { 3, "Estudar", 3 }
    };
    int i;
    int numTarefas = maxTarefas;
    printf("Lista de Tarefas (%i)", numTarefas);

    for(i = 0; i < numTarefas; i++){
        printf("\nID: %i\n" , listaDeTarefas[i].id);
        printf("Desc: %s\n" , listaDeTarefas[i].descricao);
        printf("prioridade: %i\n" , listaDeTarefas[i].prioridade);
    }
return 0;
}

