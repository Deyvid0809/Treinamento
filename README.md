    import java.util.Scanner;

class HelloWorld { public static void main(String[] args) 

{ Scanner sc = new Scanner(System.in);       

double precoa, precob, preco;
    
int quantidade, pedido, pedidoa, quantidadea;
    
String pizza, refri;
    
            System.out.println("Pizzas da Casa: ");
    System.out.println("1.Pizza Margherita Ingredientes: Molho de tomate, mussarela, manjericao fresco. Preco: R$ 25,00 ");
    System.out.println("2.Pizza Pepperoni Ingredientes: Molho de tomate, mussarela, pepperoni. Preco: R$ 28,00 ");
    System.out.println("3.Pizza Calabresa Ingredientes: Molho de tomate, mussarela, calabresa, cebola, pimentao. Preco: R$ 30,00 ");
    System.out.println("4.Pizza Frango com Catupiry Ingredientes: Molho de tomate, mussarela, frango desfiado, catupiry. Preco: R$ 32,00 ");
    System.out.println("5.Pizza Quatro Queijos Ingredientes: Molho de tomate, mussarela, queijo gorgonzola, queijo parmesao, queijo provolone. Preco: R$ 31,00 ");

    

    
    System.out.println("Qual seria o numero do peido da pizza?");
    pedido = sc.nextInt();
    
    System.out.println("Qual seria a quantidade?");
    quantidade = sc.nextInt();
    
                System.out.println("Bebidas:");
    System.out.println("1. Refrigerante (lata)Coca-Cola Preco: R$ 5.00");        
    System.out.println("2.Refrigerante (lata)Pepsi Preco: R$ 5.00");
    System.out.println("3.Refrigerante (lata)Guarana Antarctica Refrigerante Preco: R$ 5.00");
    System.out.println("4.Refrigerante (lata)Sprite Preco: R$ 5.00");
    System.out.println("5.Agua Mineral (500ml) Preco: R$ 3,00");
    
    System.out.println("Qual seria o numero do pedido da bebida?(Senao quiser colocar 0)");
    pedidoa = sc.nextInt();
    System.out.println("Qual seria a quantidade?");
    quantidadea = sc.nextInt();
    
    switch (pedido){
        case 1:
            pizza = "Pizza Margherita Ingredientes: Molho de tomate, mussarela, manjericao fresco. Preco: R$ 25,00";
            precoa = 25.00 * quantidade;
            break;
        case 2:
            pizza = "Pizza Pepperoni Ingredientes: Molho de tomate, mussarela, pepperoni. Preco: R$ 28,00";
            precoa = 28.00 * quantidade;
            break;
        case 3:
            pizza = "Pizza Calabresa Ingredientes: Molho de tomate, mussarela, calabresa, cebola, pimentao. Preco: R$ 30,00";
            precoa = 30.00 * quantidade;
            break;
        case 4:
            pizza = "Pizza Frango com Catupiry Ingredientes: Molho de tomate, mussarela, frango desfiado, catupiry.    Preco: R$ 32,00";
            precoa = 32.00 * quantidade;
            break;
        case 5:
            pizza = "Pizza Quatro Queijos Ingredientes: Molho de tomate, mussarela, queijo gorgonzola, queijo parmesao, queijo provolone. Preco: R$ 31,00";
            precoa = 31.00 * quantidade;
            break; 
        default:
            pizza = "Nenhuma";
            precoa = 00.00;
            break;
    }
    switch (pedidoa){
        case 1:
            refri = "Refrigerante (lata)Coca-Cola Preco: R$ 5.00";
            precob = 5.00 * quantidade;
            break;
        case 2:
            refri = "Refrigerante (lata)Pepsi Preco: R$ 5.00";
            precob = 5.00 * quantidade;
            break;
        case 3:
            refri = "Refrigerante (lata)Guarana Antarctica Refrigerante Preco: R$ 5.00";
            precob = 5.00 * quantidade;
            break;
        case 4:
            refri = "Refrigerante (lata)Sprite Preco: R$ 5.00";
            precob = 5.00 * quantidade;
            break;
        case 5:
            refri = "Agua Mineral (500ml) Preco: R$ 3,00";
            precob = 3.00 * quantidade;
            break; 
        default:
            refri = "Nenhuma";
            precob = 00.00;
            break;
    }
    
   preco = precoa + precob;

    if(preco == 00.00)
        System.out.println("Pedido invalido");
    else if (quantidade == 0 && quantidadea == 0)
    System.out.println("Pedido invalido");
    else{
    System.out.printf("Seu peido foi:%s%n Quantidade: %s%n %s%n Quantidade: %s%n" ,pizza,quantidade,refri,quantidadea);
    System.out.printf("Total do pedido R$ %.2f%n " ,preco);
        
    }
    
    sc.close();
    
    }
    
    
    
}
