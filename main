
package macierzprzyciskowa;
import java.awt.GridLayout;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import javax.swing.JFrame;
import javax.swing.JButton;
import javax.swing.JLabel;
import javax.swing.JPanel;
import javax.swing.JTextField;


public class MacierzPrzyciskowa extends JFrame implements ActionListener {

 //Rozmiar macierzy:
    int i=5;
    int j=6;
    
    
    private JPanel p,pp;
    private JTextField t;
    private JButton bb;
    private JLabel l;
    private JButton[][] buttons;
    private JButton b;
    
    public MacierzPrzyciskowa(){
        
     setSize(600,400);
     setTitle("Macierz");   
     
     
         p = new JPanel();
        buttons = new JButton[i][j];
        p.setLayout(new GridLayout(i, j, 3, 3));
      
       add(p);
        p.setVisible(true);
        
        pp = new JPanel();  
       pp.setVisible(false);
        
         t = new JTextField("");
       t.setBounds(100, 80, 200, 50);
            
        bb = new JButton("OK");
       bb.setBounds(160, 170, 80, 80);
       bb.addActionListener(this);
        
        for(int k=0;k<i;k++){
                for(int m=0;m<j;m++){
                         b = new JButton();
                       
                        b.setText("0");
                        p.add(b);
                        b.addActionListener(this);
                        buttons[k][m] = b;
                   }
        }      
    }
     
    Object ee;
    
    @Override
       public void actionPerformed(ActionEvent e){
           
           Object zrodlo = e.getSource();
           
           if(zrodlo == bb){
           p.setVisible(true);
           pp.setVisible(false);
           bb.setVisible(false);
          ((JButton)ee).setText(t.getText());
           }
              
           else{
           ee=  e.getSource(); 
           p.setVisible(false);
           pp.setVisible(true);
           setLayout(null);
           l = new JLabel("Podaj nowa liczbe:");
           l.setBounds(140, 10, 150, 50);
           add(l);
           add(t);
           add (bb);
           bb.setVisible(true);
           } 
    }
       
    public static void main(String[] args) {
        
       MacierzPrzyciskowa okienko = new MacierzPrzyciskowa();
       okienko.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
       okienko.setVisible(true);    
    }
}
   
