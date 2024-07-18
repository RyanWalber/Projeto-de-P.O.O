using System;

class Program
{
    static void EscolhaInvalida()
    {
        Console.WriteLine("Escolha inválida, digite novamente");
    }

    static void Pagina1()
    {
        Console.Clear();
        Console.WriteLine("-Olá capitão! Já fazem 3 semanas infernais que estamos nesse campo de batalha...");
        Console.WriteLine("-Alguns soldados observadores deram a ideia de atacar a trincheira inimiga durante a madrugada.");
        Console.WriteLine("-Eles podem está desprevenidos, ou não, se conquistarmos essa terra belga, será um grande passo para vencermos a guerra!");
        Console.WriteLine("-o que acha capitão?");
        Console.WriteLine("Não ou sim?");
        Console.WriteLine("1 - não");
        Console.WriteLine("2 - sim");
        Console.WriteLine("3 - Pensar...");

        int escolha = int.Parse(Console.ReadLine());

        if (escolha == 1)
        {
            Pagina2();
        }
        else if (escolha == 2)
        {
            Pagina3();
        }
        else if (escolha == 3)
        {
            Pagina4();
        }
        else
        {
            EscolhaInvalida();
        }
    }

    static void Pagina2()
    {
        Console.Clear();
        Console.WriteLine("-Certo, então não atacaremos! até porque seria bem desleal...");
        Console.WriteLine("-Capitão!! Estão nos atacando! É madrugada, estávamos um pouco despreparados...");
        Console.WriteLine("-O que devemos fazer?!");
        Console.WriteLine("1 - Recuar");
        Console.WriteLine("2 - Lutar");
        

        // O usuário precisa digitar o número da sua escolha
        int escolha = int.Parse(Console.ReadLine());

        if (escolha == 1)
        {
            Pagina6();
        }
        else if (escolha == 2)
        {
            Pagina7();
        }
        else
        {
            EscolhaInvalida();
        }
    }

    static void Pagina3()
    {
        Console.Clear();
        Console.WriteLine("-Certo capitão! Atacaremos durante a madrugada...");
        Console.WriteLine("-Nós atacamos, porém já estavam a nossa espera! Estamos em uma enorme desvantagem!");
        Console.WriteLine("-Nos ajude, o que devemos fazer?");
        Console.WriteLine("1 - Lutar");
        Console.WriteLine("2 - Fugir");

        int escolha = int.Parse(Console.ReadLine());

        if (escolha == 1)
        {
            Pagina5();
        }
        else if (escolha == 2)
        {
            Pagina7();
        }
        else
        {
            EscolhaInvalida();
        }
    }

    static void Pagina4()
    {
        Console.Clear();
        Console.WriteLine("-Pensamos demais... Eles nos atacaram!!!");
        Console.WriteLine("1 - Lutar");

        int escolha = int.Parse(Console.ReadLine());

        if (escolha == 1)
        {
            Pagina5();
        }
        
    }

    static void Pagina5()
    {
        Console.Clear();
        Console.WriteLine("-Infelizmente não fomos fortes o suficiente... Foi bom lutar ao lado capitão! GAME OVER.");
    }

    static void Pagina6()
    {
        Console.Clear();
        Console.WriteLine("-Bom... Recuamos e perdemos muitas terras importantes, porém pelo menos alguns de nós sobrevivemos... Tivemos um final humilhante capitão.");
    }
    static void Pagina7()
    {
        Console.Clear();
        Console.WriteLine("-Outro batalhão ficou sabendo da nossa batalha! E vinheram nos dar apoio.");
        Console.WriteLine("-O que devemos fazer capitão!");
        Console.WriteLine("1 - Ficar e lutar!");
        Console.WriteLine("2 - Fugir");

        int escolha = int.Parse(Console.ReadLine());

        if (escolha == 1)
        {
            Pagina8();
        }
        else if (escolha == 2)
        {
            Pagina6();
        }
        else
        {
            EscolhaInvalida();
        }
    }

    static void Pagina8()
    {
        Console.Clear();
        Console.WriteLine("-Vamos ficar! Qual estratégia devemos usar contra os inimigos, para sermos mais efetivos?");
        Console.WriteLine("1 - Ir de frente!");
        Console.WriteLine("2 - Encurralar eles.");

        int escolha = int.Parse(Console.ReadLine());
        if (escolha == 1)
        {
            Pagina9();
        }
        else if (escolha == 2)
        {
            Pagina11();
        }
        else
        {
            EscolhaInvalida();
        }
    }

    static void Pagina9()
    {
        Console.Clear();
        Console.WriteLine("-Capitão! Tem um inimigo atrás do senhor! Pegue alguma arma e lute!");
        Console.WriteLine("O que vai pegar?");
        Console.WriteLine("1 - Arma de fogo");
        Console.WriteLine("2 - Punhal");

        int escolha = int.Parse(Console.ReadLine());

        if (escolha == 1)
        {
            Pagina10();
        }
        else if (escolha == 2)
        {
            Pagina12();
        }
        else
        {
            EscolhaInvalida();
        }
    }

    static void Pagina10()
    {
        Console.Clear();
        Console.WriteLine("-Capitão... Capitão... Foi uma honra lutar ao seu lado, só ganhamos por sua causa.");
        Console.WriteLine("Final bom? Sua arma estava sem munição e você morreu... Mas seu batalhão ganhou a Batalha!");
    }
static void Pagina11()
    {
        Console.Clear();
        Console.WriteLine("-Muito bem capitão! Ganhamos a batalha com poucas baixas, parabéns! Com certeza ajudamos nossa pátria, e fomos heróis!");
        Console.WriteLine("Parabéns guiou sua equipe para a vitória! Muito bem.");
        Console.WriteLine("FIM");
    }
static void Pagina12()
    {
        Console.Clear();
        Console.WriteLine("-Muito bem capitão! Ganhamos a batalha com poucas baixas, parabéns! Com certeza ajudamos nossa pátria, e fomos heróis!");
        Console.WriteLine("Vocês lutaram muito, que bom que você sabia lutar corpo a corpo e usar uma faca, para que uma arma né? Enfim você saiu vivo, só com pequenos arranhões e conseguiram derrotar o batalhão inimigo, e conquistaram uma terra muito importante, deram um enorme passo para ganharem a guerra.");
        Console.WriteLine("FIM");
    }
    static void Main()
    {
        Pagina1();
    }
}
