# include <stdio.h>
struct Carta {
  char estado;
  char codigo[4];
  char nomeCidade[50];
  int populacao;
  float area;
  float pib;
  int pontosTuristicos;
  };



int main() {
  struct Carta carta1;
  struct Carta carta2;


  // -----------------------------------------------------------------------------
  // BLOCO DE ENTRADA DE DADOS - CARTA 1
  // -----------------------------------------------------------------------------

  printf("--- Cadastro da Carta 1 ---\n");
  
  printf("Digite o Estado (uma letra de 'A' a 'H'): ");
  scanf(" %c", &carta1.estado);

  printf("Digite o Codigo da Carta (ex: A01): ");
  scanf("%s", carta1.codigo);

  printf("Digite o Nome da Cidade (use '_' para espacos, ex: Rio_de_Janeiro): ");
  scanf("%s", carta1.nomeCidade);

  printf("Digite a Populacao da cidade: ");
  scanf("%d", &carta1.populacao);

  printf("Digite a Area da cidade (em km2): ");
  scanf("%f", &carta1.area);

  printf("Digite o PIB da cidade (em bilhoes): ");
  scanf("%f", &carta1.pib);

  printf("Digite o Numero de Pontos Turisticos: ");
  scanf("%d", &carta1.pontosTuristicos);

  printf("\n"); // Adiciona uma linha em branco para melhorar a legibilidade no terminal.


  // -----------------------------------------------------------------------------
  // BLOCO DE ENTRADA DE DADOS - CARTA 2
  // ----------------------------------------------------------------------------

  printf("--- Cadastro da Carta 2 ---\n");

  printf("Digite o Estado (uma letra de 'A' a 'H'): ");
  scanf(" %c", &carta2.estado);

  printf("Digite o Codigo da Carta (ex: B02): ");
  scanf("%s", carta2.codigo);

  printf("Digite o Nome da Cidade (use '_' para espacos, ex: Belo_Horizonte): ");
  scanf("%s", carta2.nomeCidade);

  printf("Digite a Populacao da cidade: ");
  scanf("%d", &carta2.populacao);

  printf("Digite a Area da cidade (em km2): ");
  scanf("%f", &carta2.area);

  printf("Digite o PIB da cidade (em bilhoes): ");
  scanf("%f", &carta2.pib);

  printf("Digite o Numero de Pontos Turisticos: ");
  scanf("%d", &carta2.pontosTuristicos);

  printf("\n\n"); // Adiciona duas linhas em branco para separar a entrada da saída.


  // -----------------------------------------------------------------------------
  // BLOCO DE EXIBIÇÃO DOS DADOS CADASTRADOS
  // -----------------------------------------------------------------------------

  printf("======================================\n");
  printf("    DADOS DAS CARTAS CADASTRADAS    \n");
  printf("======================================\n\n");

  // Exibe os dados da Carta 1 de forma organizada
  printf("Carta 1:\n");
  printf("Estado: %c\n", carta1.estado);
  printf("Codigo: %s\n", carta1.codigo);
  printf("Nome da Cidade: %s\n", carta1.nomeCidade);
  printf("Populacao: %d\n", carta1.populacao);
  printf("Area: %.2f km2\n", carta1.area);
  printf("PIB: %.2f bilhoes de reais\n", carta1.pib);
  printf("Numero de Pontos Turisticos: %d\n", carta1.pontosTuristicos);

  printf("\n"); // Linha em branco para separar a exibição das duas cartas.

  // Exibe os dados da Carta 2 de forma organizada
  printf("Carta 2:\n");
  printf("Estado: %c\n", carta2.estado);
  printf("Codigo: %s\n", carta2.codigo);
  printf("Nome da Cidade: %s\n", carta2.nomeCidade);
  printf("Populacao: %d\n", carta2.populacao);
  printf("Area: %.2f km2\n", carta2.area);
  printf("PIB: %.2f bilhoes de reais\n", carta2.pib);
  printf("Numero de Pontos Turisticos: %d\n", carta2.pontosTuristicos);



  return 0;
  }
