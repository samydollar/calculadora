# calculadora
calculdora.java.grafi



using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Windows.Forms;

namespace Calculadora
{
    public partial class Form1 : Form
    {
        double a;
        double b;
        double res;
        string opera;
        public Form1()
        {
            InitializeComponent();
        }
        private void button11_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '0';
        }
        private void button1_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '1';
        }
        private void button2_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '2';
        }
        private void button3_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '3';
        }
        private void button4_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '4';
        }
        private void button5_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '5';
        }
        private void button6_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '6';
        }
        private void button7_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '7';
        }
        private void button8_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '8';
        }
        private void button9_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '9';
        }
        private void button10_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + '.';
        }
        private void botsuma_Click(object sender, EventArgs e)
        {
            opera = "+";
            a = double.Parse(textBox1.Text);
            textBox1.Clear();
        }
        private void botresta_Click(object sender, EventArgs e)
        {
            opera = "-";
            a = double.Parse(textBox1.Text);
            textBox1.Clear();
        }
        private void botdiv_Click(object sender, EventArgs e)
        {
            opera = "/";
            a = double.Parse(textBox1.Text);
            textBox1.Clear();
        }
        private void botmulti_Click(object sender, EventArgs e)
        {
            opera = "*";
            a = double.Parse(textBox1.Text);
            textBox1.Clear();
        }
        private void button13_Click(object sender, EventArgs e)
        {
            opera = "raiz";
            a = double.Parse(textBox1.Text);
            res = a;
            textBox1.Text = Math.Sqrt(a).ToString();
        }
        private void botcuadrado_Click(object sender, EventArgs e)
        {
            opera = "^";
            a = double.Parse(textBox1.Text);
            textBox1.Clear();
        }
        private void button12_Click(object sender, EventArgs e)
        {
            b = double.Parse(textBox1.Text);
            switch (opera)
            {
                case "+":
                    res = a + b;
                    textBox1.Text = res.ToString();
                    break;
                case "-":
                    res = a - b;
                    textBox1.Text = res.ToString();
                    break;
                case "*":
                    res = a * b;
                    textBox1.Text = res.ToString();
                    break;
                case "/":
                    res = a / b;
                    textBox1.Text = res.ToString();
                    break;
                case "^":
                    res = Math.Pow(a, b);
                    textBox1.Text = res.ToString();
                    break;
            }
        }
        private void button17_Click(object sender, EventArgs e)
        {
            textBox1.Clear();
        }
    }
}
