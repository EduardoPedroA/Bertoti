Engenharia de Software



Ciclo de vida



Requisitos



Funcionais
![WhatsApp Image 2022-03-11 at 18 56 04](https://user-images.githubusercontent.com/90360441/157979278-6a4d05f7-d857-4dce-8aae-07c65a7a9591.jpeg)

Storycard
![WhatsApp Image 2022-03-14 at 19 08 24](https://user-images.githubusercontent.com/90360441/158269290-83d81da8-ec97-418c-9cd1-bb5945cabcda.jpeg)




Não Funcionais

 ![image](https://user-images.githubusercontent.com/90360441/157985208-76d5c509-41f3-46c0-93fd-adced1a4ad45.png)
 
Mostra que a mensagem foi visualizada, que entra na 1ª Heurística

![image](https://user-images.githubusercontent.com/90360441/157985504-3f232d53-0e21-4f7c-8589-be531a32dfed.png)

Cada ícone mostra pra onde vai, ajudando a facilitar o entendimento da plataforma, que entra na 2ª Heurística

![image](https://user-images.githubusercontent.com/90360441/157985546-81195403-6b28-4f75-9a08-0f5e4acf4c36.png)
 
Da uma opção de voltar direto para onde o usuário estava, que entra na 3ª Heurística

![image](https://user-images.githubusercontent.com/90360441/157985572-39e11f97-78e7-486a-b948-416026e32aa0.png)

Ter a função de pesquisa ajuda ao usuário a encontrar mais fácil o que ele procura, o que entra na 4ª Heurística

![image](https://user-images.githubusercontent.com/90360441/157985586-a142610b-91ca-498d-9859-d0ea2c97399d.png)

A opção de ajuda da uma saída para o usuário se orientar sobre algo que não consegue fazer, que entra na Heurística 10



Atividade 2 (Projeto Diagrama)

![WhatsApp Image 2022-04-25 at 19 19 46 (1)](https://user-images.githubusercontent.com/90360441/165184685-442e9867-6057-407e-a0f7-d1c4cd9e0d1c.jpeg)
![WhatsApp Image 2022-04-25 at 19 19 46](https://user-images.githubusercontent.com/90360441/165184704-72347cbc-ee12-4b73-8cef-fe392775466c.jpeg)

Densenvolvimento

Plataforma de Ensino/Main

package Plataforma_de_Ensinoo;

import java.util.LinkedList;
import java.util.List;

public class Plataforma {

     private List<Pessoa> pessoa = new LinkedList<Pessoa>();

     public void cadastrarPessoa(Pessoa pessoa){
          pessoa.add(pessoa);
     }

     public List<Pessoa> buscarPessoaPorDiciplina(Diciplina Materia){
           List<Pessoa> pessoasEncontrados = new LinkedList<Pessoa>();
           Pessoa[] pessoas = null;
		for(Pessoa pessoa:pessoas){
                if(pessoa.getDiciplina().comparar(Materia)) pessoasEncontrados.add(pessoa);
           }
           return pessoasEncontrados;
     }

     public Pessoa buscarpessoaPorCPF(String CPF){
          Pessoa[] pessoas = null;
		for(Pessoa pessoa:pessoas){
			if(pessoa.getPessoa().equals(getPessoa())) return pessoa; 
          }
          return null;
     }

     public List<Pessoa> getPessoa(){
           List<Pessoa> pessoas = null;
		return pessoas;
     }
}

Plataforma de Ensino/Pessoa

package Plataforma_de_Ensinoo;

public class Pessoa {
	
	
	
	private String Pessoa;
	private String Turma;
	private int RA;
	private String Data_de_Nascimento;
	private int CPF;
	
	public Pessoa (String Pessoa, String Turma, int RA, String Data_de_nascimento, int CPF) {
		this.Pessoa = Pessoa;
		this.Turma = Turma;
	}

	public String getPessoa(){
		return Pessoa;
	}
	
	public void setPessoa(String novaPessoa) {
		Pessoa = novaPessoa;
	}
	
	public String getTurma() {
		return Turma;
	}
	
	public void setTurma(String novaTurma) {
		Turma = novaTurma;
	}
	
	public int getRA() {
		return RA;
	}
	
	public void setRA(int novaRA) {
		RA = novaRA;
	}
	
	public String getData_de_Nascimento(){
		return Data_de_Nascimento;
	}
	
	public void setData_de_Nascimento(String novaData_de_Nascimento) {
		Data_de_Nascimento = novaData_de_Nascimento;
	}
	

	
	public int getCPF(){
		return CPF;
	}

	public void setCPF(int novaCPF) {
		this.CPF = novaCPF;



}

	public void add(Pessoa pessoa2) {
		
		
	}

	public Diciplina getDiciplina() {
		// TODO Auto-generated method stub
		return null;
	}
	}
 
 Plataforma/Diciplina
 
 package Plataforma_de_Ensinoo;

public class Diciplina {
	
	private String Materia;
	private String Professor;
	private String Turma;

	public Diciplina(String Materia, String Professor, String Turma) {
		this.Materia = Materia;
		this.Professor = Professor;
		this.Turma = Turma;
	}
	
	public String getMarca() {
		return Materia;
	}
	
	public void setMateria(String novaMateria) {
		this.Materia = novaMateria;
	}
	
	public String getProfessor() {
		return Professor;
	}
	
	public void setProfessor(String novoProfessor) {
		this.Professor= novoProfessor;
	}
	
	public String getTurmaPessoa() {
		return Turma;
	}
	
	public void setTurmaPessoa(String Turma) {
		this.Turma = Turma;
	}
	
	public boolean comparar(Diciplina Diciplina){
		if(this.Materia.equals(Diciplina.Materia) &&            					this.Professor.equals(Diciplina.Professor) 
				&& 					this.Turma.equals(Diciplina.Turma)){
			return true;
		} else {
			return false;
		}
	}


}









