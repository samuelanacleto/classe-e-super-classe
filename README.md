# classe-e-super-classe
public class funcionario {
	private String nome;
	private double salario;
	
	
	public String GetNome(){
		return this.nome;}
	
	public void SetNome(String nome){
		this.nome=nome;}
	
	public double getSalario(){
		return this.salario;}
	public void SetSalario(double salario){
		this.salario=salario;}
	public double  calculaBonificaçao(){
		return this.salario*0.1;}
	}
  |||||||||||||||||||||||||||||||||||||||||
  public class gerente extends funcionario{
	private String usuario;
	private String senha;
	
	public void setUsuario(String usuario){
		this.usuario=usuario;}
	public String getUsuario(){
		return this.usuario;}
	
	public String getSenha(){
		return this.senha;}
	public void setSenha (String senha){
		this.senha=senha;}
	public double  calculaBonificação(){
		return this.salario*0.6+100;}
}
|||||||||||||||||||||||||||||||||||||||||
public class testaFuncionario {
	public static void main (String [] args){
		funcionario f = new funcionario();
		f.setNome("pedro castelo");
		f.setSalario(1500);
		
		gerente g = new gerente ();
		g.setNome("Carlos vieira");
		g.setSalario(3000);
		g.setUsuario("carlos vieira");
		g.setSenha("12345");
		System.out.println("##funcionario##"); 
		System.out.println("Nome:"+f.getNome());
		System.out.println("salario:"+f.getSalario());
		System.out.println("bonificação:"+f.calculaBonificaçao());
		System.out.println();
		System.out.println("##Gerente##"); 
		System.out.println("Nome:"+g.getNome());
		System.out.println("salario:"+g.getSalario());
		System.out.println("bonificação:"+g.calculaBonificaçao());
		System.out.println();
		}}
    
    |||||||||||||||||||||||||||||||||||||||||||||||
