
import java.awt.BorderLayout;
import java.awt.Button;
import java.awt.Color;
import java.awt.Font;
import java.awt.Frame;
import java.awt.GridLayout;
import java.awt.Menu;
import java.awt.MenuBar;
import java.awt.MenuItem;
import java.awt.Panel;
import java.awt.TextField;
import java.awt.Toolkit;
import java.awt.datatransfer.Clipboard;
import java.awt.datatransfer.DataFlavor;
import java.awt.datatransfer.StringSelection;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;
import java.io.IOException;

class Close extends WindowAdapter {

    public void windowClosing(WindowEvent e) {
        System.exit(0);
    }
}

class Cal implements ActionListener {
// add buttons objects

    Button b1, b2, b3, b4, b5, b6, b7, b8, b9, b10, b11, b12, b13, b14, b15, b16, b17, b18, b19, b20, b21, b22, b23, b24, b25;

// add textfield objects
    TextField tf;

    String fv, sv, op;
    double fdv, sdv, tot;

    Cal() {
        Frame f1 = new Frame();
        f1.setBackground(Color.WHITE);
        f1.addWindowListener(new Close());
        f1.setBounds(500, 200, 300, 400); // set the bounds of the frame
        f1.setTitle("Calculator");

        MenuBar mbar = new MenuBar();
        Menu m1 = new Menu("Layout");
        MenuItem mi1 = new MenuItem("Standard");
        MenuItem mi2 = new MenuItem("Scientific");
        m1.add(mi1);
        m1.add(mi2);

        Menu m2 = new Menu("Edit");
        MenuItem mi3 = new MenuItem("Copy");
        MenuItem mi4 = new MenuItem("Paste");
        mi3.addActionListener(this);
        mi4.addActionListener(this);
        m2.add(mi3);
        m2.add(mi4);

        Menu m3 = new Menu("Help");
        MenuItem mi5 = new MenuItem("Help");
        MenuItem mi6 = new MenuItem("About");
        m3.add(mi5);
        m3.add(mi6);

        Menu m4 = new Menu("View");
        MenuItem mi7 = new MenuItem("Light");
        MenuItem mi8 = new MenuItem("Dark");
        m4.add(mi7);
        m4.add(mi8);

        mbar.add(m1);
        mbar.add(m2);
        mbar.add(m3);
        mbar.add(m4);

        f1.setMenuBar(mbar);

        b1 = new Button("C");
        b2 = new Button("CE");
        b3 = new Button("%");
        b4 = new Button("/");

        b5 = new Button("7");
        b6 = new Button("8");
        b7 = new Button("9");
        b8 = new Button("*");

        b9 = new Button("4");
        b10 = new Button("5");
        b11 = new Button("6");
        b12 = new Button("-");

        b13 = new Button("1");
        b14 = new Button("2");
        b15 = new Button("3");
        b16 = new Button("+");

        b17 = new Button("+/-");
        b18 = new Button("0");
                
        p2.add(b17);
        p2.add(b18);
        p2.add(b19);
        p2.add(b20);

        f1.add(tf, BorderLayout.NORTH);
        f1.add(p1, BorderLayout.CENTER);
        f1.add(p2, BorderLayout.SOUTH);

        f1.setVisible(true);

    }

    public void actionPerformed(ActionEvent e) {

        String s = e.getActionCommand();

        if (s.equals("1")) {
            fv = tf.getText();
            tf.setText(fv + "1");
        }

        if (s.equals("2")) {
            fv = tf.getText();
            tf.setText(fv + "2");
        }

        if (s.equals("3")) {
            fv = tf.getText();
            tf.setText(fv + "3");
        }

        if (s.equals("4")) {
            fv = tf.getText();
            tf.setText(fv + "4");
        }

        if (s.equals("5")) {
            fv = tf.getText();
            tf.setText(fv + "5");
        }

        if (s.equals("6")) {
            fv = tf.getText();
            tf.setText(fv + "6");
        }

        if (s.equals("7")) {
            fv = tf.getText();
            tf.setText(fv + "7");
        }

        if (s.equals("8")) {
            fv = tf.getText();
            tf.setText(fv + "8");
        }

        if (s.equals("9")) {
            fv = tf.getText();
            tf.setText(fv + "9");
        }

        if (s.equals("0")) {
            fv = tf.getText();
            tf.setText(fv + "0");
        }

        if (s.equals("+")) {
            fv = tf.getText();
            op = "+";
            tf.setText("");
        }

        if (s.equals("-")) {
            fv = tf.getText();
            op = "-";
            tf.setText("");
        }

        if (s.equals("*")) {
            fv = tf.getText();
            op = "*";
            tf.setText("");
        }

        if (s.equals("/")) {
            fv = tf.getText();
            op = "/";
            tf.setText("");
        }

        if (s.equals(".")) {
            fv = tf.getText();
            tf.setText(fv + ".");
        }

        if (s.equals("%")) {
            fv = tf.getText();
            op = "%";
            tf.setText("");
        }

        if (s.equals("+/-")) {
            fv = tf.getText();
            if (fv.charAt(0) == '-') {
                tf.setText(fv.substring(1));
            } else {
                tf.setText("-" + fv);
            }
        }

        if (s.equals("=")) {
            sv = tf.getText();
            fdv = Double.parseDouble(fv);
            sdv = Double.parseDouble(sv);

            if (op.equals("+")) {
                tot = fdv + sdv;
            }

            if (op.equals("-")) {
                tot = fdv - sdv;
            }

            if (op.equals("*")) {
                tot = fdv * sdv;
            }

            if (op.equals("/")) {
                tot = fdv / sdv;
            }

            if (op.equals("%")) {
                tot = fdv % sdv;
            }

            tf.setText(String.valueOf(tot));
        }

        if (s.equals("C")) {
            tf.setText("");
        }

        if (s.equals("CE")) {
            tf.setText("");
        }
    }
}

public class Calculator {

    public static void main(String[] args) {

        new Cal();

    }
}
