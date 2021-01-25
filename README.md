# LG2_pilha_fila
exemplos dos vídeos

/Código da classe Pilha/

import java.util.LinkedList;
import java.util.List;

public class Pilha {
	private List<String> nomes = new LinkedList<String>();
	
	public void push(String nome) {
		nomes.add(nome);
	}
	
	public String pop() {
		return nomes.remove(nomes.size()-1);
	}
	
	public boolean vazia() {
		return nomes.isEmpty();
	}
	
	public String toString() {
		return nomes.toString();
	}
}

/Código fonte para testar a classe Pilha/

import java.util.Stack;

public class TesteDaPilha {

	public static void main(String[] args) {
		Pilha pilha = new Pilha();
		
		pilha.push("Mauricio");
		System.out.println(pilha);
		
		pilha.push("Guilherme");
		System.out.println(pilha);
		
		String r1 = pilha.pop();
		System.out.println(r1);
	
		String r2 = pilha.pop();
		System.out.println(r2);
		
		System.out.println(pilha.vazia());
		pilha.push("Marcelo");
		System.out.println(pilha.vazia());
		
		System.out.println(pilha);
		
		Stack<String> stack = new Stack<String>();
		stack.push("Mauricio");
		stack.push("Guilherme");
		
		System.out.println(stack);
		
		System.out.println(stack.pop());
		
		System.out.println(stack);
		
		String nome = stack.peek();
		System.out.println(nome);
		
		System.out.println(stack);
	}
}

*Código da classe Fila*

import java.util.LinkedList;
import java.util.List;

public class Fila {
	private List<String> alunos = new LinkedList<String>();
	
	public void adiciona(String aluno) {
		alunos.add(aluno);
	}
	
	public String remove() {
		return alunos.remove(0);
	}
	
	public boolean vazio() {
		return alunos.isEmpty();
	}
	
	public String toString() {
		return alunos.toString();
	}
}

*Código fonte para testar a classe Fila*

import java.util.LinkedList;
import java.util.Queue;

public class TesteFila {

	public static void main(String[] args) {

		FIla fila = new Fila();
		
		fila.adiciona("Mauricio");
		fila.adiciona("Guilherme");
		
		System.out.println(fila);
		
		String x1 = fila.remove();
		
		System.out.println(x1);
		System.out.println(fila);
		
		Queue<String> FilaDoJava = new LinkedList<String>();
		
		FilaDoJava.add("Mauricio");
		String x2 = FilaDoJava.poll();
		
		System.out.println(x2);
	}

}
