  ArrayList<String> nomes = new ArrayList<String>(1);
        nomes.add("Ana");
        nomes.add("Bruno");
        nomes.add("Carlos");
        nomes.add("Daniela");
        nomes.add("Eduardo");
        nomes.add("Fernanda");
        nomes.add("Gabriel");
        nomes.add("Helena");
        int contador = 1;
        for(String nome : nomes){
            System.out.printf("O %dº nome é: %s\n",contador,nome);contador++;
        }
  ------------- ou ---------------
  
   ArrayList<String> nomes= new ArrayList<String>(Arrays.asList("vitu","leo","Ana","Bruno","Carlos","Daniela","Eduardo","Fernanda","Gabriel","Helena"));
   for(String nome : nomes)System.out.printf("Próximo nome: %s\n",nome);
  
  //2- ArrayList<String> nomes= new ArrayList<String>(4);
        for (int i = 0;i<4;i++){
            System.out.println("informe o prox nome: ");
            nomes.add(sc.nextLine());
        }
        for(String nome: nomes) System.out.println("Prox nome: "+nome);
     
