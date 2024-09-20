# contas
import java.sql.SQLOutput;

public class Livro {
    private String titulo;
    private String autor;
    private int anoPublicado;
    private boolean emprestado;
    private boolean devolver;

    public Livro(String titulo, String autor, int anoPublicado) {
        this.titulo = titulo;
        this.autor = autor;
        this.anoPublicado = anoPublicado;
        this.emprestado = false;
    }

    public void emprestar() {
        if (this.emprestado == false) {
            this.emprestado = true;
        }
    }

    public void devolver(){
        if(this.emprestado == true)
            this.emprestado= false;
    }

    public void exibirInformações(){
        System.out.println(titulo + autor + anoPublicado + emprestado + devolver);
    }
}
