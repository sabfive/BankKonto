
import java.util.ArrayList;


public class BankKonto {

    public static void main(String[] args) {
    
    private String kontoNamn;
    private int kontoNr;
    private double kontoSaldo;     

    public BankKonto() {
    	this.kontoNamn = null;
    	this.kontoNr = 0;
    	this.kontoSaldo = 0;
    }
    public BankKonto(String namn , int nr, double saldo) {
    	this.kontoNamn = namn;
    	this.kontoNr = nr;
    	this.kontoSaldo = saldo;
    }
    
    // Metoder för att sätta värden
    public void setNr(int nr) {
       kontoNr = nr;
    }
    
    public void setNamn(String namn) {
        kontoNamn = namn;
    }
    
    public void setSaldo(double saldo) {
         kontoSaldo = saldo;
    }
    
    // Metoder som returnerar värden
    public int getNr() {
        return kontoNr = 0;
    }
    
     public String getNamn() {     
        return kontoNamn = null;
    } 
 
    public double getsaldo() {
        return kontoSaldo = 0; 
    }
    
    //Sriver ut information om konto på skärmen
    public void skrivUtKonto() {

        
    }

       ArrayList<BankKonto> bankKontoList = new ArrayList<BankKonto>();
    
        public boolean newbankKont(int nr, String namn, double saldo){
        BankKonto newBankKonto = new BankKonto();    

        newBankKonto.kontoNr = nr;
        newBankKonto.kontoNamn = namn;
        newBankKonto.kontoSaldo = saldo;
        
        bankKontoList.add(newBankKonto);
        
        return true;
    }
    
    public void mainshowAllBankKonto(){
        System.out.println("Kontonummer: \t Personnummer: \t Namn: \t Saldo \t");
        for(int i = 0; i < bankKontoList.size(); i++){
            System.out.println(
                    bankKontoList.get(i).kontoNr + "\t" +
                    bankKontoList.get(i).kontoNamn + "\t" +
                    bankKontoList.get(i).kontoSaldo + "\t");
                }
            }
}
