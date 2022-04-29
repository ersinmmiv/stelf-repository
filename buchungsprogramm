import java.awt.Color;
import java.awt.EventQueue;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.text.DecimalFormat;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPanel;
import javax.swing.JTextField;
import javax.swing.SwingConstants;
import javax.swing.border.EmptyBorder;
import javax.swing.DropMode;

//Julius stinkt hart nach Maggi

@SuppressWarnings("serial")
public class buchungsprogramm extends JFrame implements ActionListener {

	double zahl1 = 0, zahl2 = 0, ergebnis = 0;

	public static final DecimalFormat df = new DecimalFormat("0.00");
	
	public int[][] Buchungen = new int[10][3];
		
	private JPanel contentPane;
	private JTextField txtNumberOne;
	private JLabel lblNumberOne;
	private JLabel lblNumberTwo;
	private JTextField txtNumberTwo;
	private JTextField txtNumberThree;
	private JButton btnBuchen;
	private JLabel lblWieVielePersonen;
	private JTextField txtNumberFour;
	private JLabel lblWelcherBungalowSoll;
	private JTextField txtNumberFive;
	private JTextField txtNumberSix;
	private JButton btnAnzeigen;
	private JTextField txtNumberSeven;
	private JTextField txtNumberEight;

	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					buchungsprogramm frame = new buchungsprogramm();
					frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	public buchungsprogramm() {

		setBackground(new Color(0, 0, 0));
		setForeground(new Color(255, 255, 255));
		setTitle("Buchung");
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setBounds(200, 100, 600, 350);
		contentPane = new JPanel();
		contentPane.setBackground(new Color(51, 51, 51));
		contentPane.setForeground(Color.BLACK);
		contentPane.setBorder(new EmptyBorder(5, 5, 5, 5));
		setContentPane(contentPane);
		contentPane.setLayout(null);

		lblNumberOne = new JLabel("Nummer des Bungalows(1-10):");
		lblNumberOne.setForeground(Color.WHITE);
		lblNumberOne.setBackground(Color.WHITE);
		lblNumberOne.setBounds(27, 35, 145, 23);
		contentPane.add(lblNumberOne);

		txtNumberOne = new JTextField();
		txtNumberOne.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberOne.setForeground(new Color(255, 255, 255));
		txtNumberOne.setBackground(Color.MAGENTA);
		txtNumberOne.setBounds(182, 36, 118, 20);
		contentPane.add(txtNumberOne);
		txtNumberOne.setColumns(10);

		lblNumberTwo = new JLabel("Start Kalenderwoche (1-51):");
		lblNumberTwo.setForeground(Color.WHITE);
		lblNumberTwo.setBounds(27, 69, 145, 25);
		contentPane.add(lblNumberTwo);

		txtNumberTwo = new JTextField();
		txtNumberTwo.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberTwo.setForeground(new Color(255, 255, 255));
		txtNumberTwo.setBackground(Color.MAGENTA);
		txtNumberTwo.setBounds(182, 71, 118, 20);
		contentPane.add(txtNumberTwo);
		txtNumberTwo.setColumns(10);
		JLabel lblEndeKalenderwoche = new JLabel("Ende Kalenderwoche (1-51):");
		lblEndeKalenderwoche.setForeground(Color.WHITE);
		lblEndeKalenderwoche.setBounds(27, 104, 145, 25);
		contentPane.add(lblEndeKalenderwoche);
		txtNumberThree = new JTextField();
		txtNumberThree.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberThree.setForeground(Color.WHITE);
		txtNumberThree.setColumns(10);
		txtNumberThree.setBackground(Color.MAGENTA);
		txtNumberThree.setBounds(182, 107, 118, 20);
		contentPane.add(txtNumberThree);
		btnBuchen = new JButton("Buchen");
		btnBuchen.setForeground(Color.BLACK);
		btnBuchen.addActionListener(this);
		btnBuchen.setBackground(Color.RED);
		btnBuchen.setBounds(110, 190, 110, 25);
		contentPane.add(btnBuchen);
		
		lblWieVielePersonen = new JLabel("WIe viele Personen");
		lblWieVielePersonen.setForeground(Color.WHITE);
		lblWieVielePersonen.setBounds(27, 139, 145, 25);
		contentPane.add(lblWieVielePersonen);
		
		txtNumberFour = new JTextField();
		txtNumberFour.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberFour.setForeground(Color.WHITE);
		txtNumberFour.setColumns(10);
		txtNumberFour.setBackground(Color.MAGENTA);
		txtNumberFour.setBounds(182, 142, 118, 20);
		contentPane.add(txtNumberFour);
		
		lblWelcherBungalowSoll = new JLabel("Welcher Bungalow soll angezeigt werden");
		lblWelcherBungalowSoll.setForeground(Color.WHITE);
		lblWelcherBungalowSoll.setBackground(Color.WHITE);
		lblWelcherBungalowSoll.setBounds(376, 40, 200, 35);
		contentPane.add(lblWelcherBungalowSoll);
		
		txtNumberFive = new JTextField();
		txtNumberFive.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberFive.setForeground(Color.WHITE);
		txtNumberFive.setColumns(10);
		txtNumberFive.setBackground(Color.MAGENTA);
		txtNumberFive.setBounds(411, 72, 118, 20);
		contentPane.add(txtNumberFive);
		
		txtNumberSix = new JTextField();
		txtNumberSix.setDropMode(DropMode.INSERT);
		txtNumberSix.setEditable(false);
		txtNumberSix.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberSix.setForeground(Color.WHITE);
		txtNumberSix.setColumns(10);
		txtNumberSix.setBackground(Color.PINK);
		txtNumberSix.setBounds(411, 142, 118, 20);
		contentPane.add(txtNumberSix);
		
		btnAnzeigen = new JButton("Anzeigen");
		btnAnzeigen.setForeground(Color.BLACK);
		btnAnzeigen.setBackground(Color.RED);
		btnAnzeigen.setBounds(411, 106, 118, 25);
		contentPane.add(btnAnzeigen);
		btnAnzeigen.addActionListener(this);
		
		txtNumberSeven = new JTextField();
		txtNumberSeven.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberSeven.setForeground(Color.WHITE);
		txtNumberSeven.setColumns(10);
		txtNumberSeven.setBackground(Color.PINK);
		txtNumberSeven.setBounds(411, 172, 118, 20);
		contentPane.add(txtNumberSeven);
		
		txtNumberEight = new JTextField();
		txtNumberEight.setHorizontalAlignment(SwingConstants.CENTER);
		txtNumberEight.setForeground(Color.WHITE);
		txtNumberEight.setColumns(10);
		txtNumberEight.setBackground(Color.PINK);
		txtNumberEight.setBounds(411, 202, 118, 20);
		contentPane.add(txtNumberEight);
	}

	@Override
	public void actionPerformed(ActionEvent e) {
		if(e.getSource()==btnBuchen) {
				Buchungen[Integer.parseInt(txtNumberOne.getText())][0] = Integer.parseInt(txtNumberTwo.getText());
				Buchungen[Integer.parseInt(txtNumberOne.getText())][1] = Integer.parseInt(txtNumberThree.getText());
				Buchungen[Integer.parseInt(txtNumberOne.getText())][2] = Integer.parseInt(txtNumberFour.getText());
			}
		
		if(e.getSource()==btnAnzeigen) {
			txtNumberSix.setText("Anfangsmonat: " + Buchungen[Integer.parseInt(txtNumberFive.getText())][0]);
			txtNumberSeven.setText("Endemonat: " + Buchungen[Integer.parseInt(txtNumberFive.getText())][1]);
			txtNumberEight.setText("Anzahl Personen: " + Buchungen[Integer.parseInt(txtNumberFive.getText())][2]);
		}
		
	}
}
