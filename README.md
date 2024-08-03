# CAR-DETAILS-using-classes-in-Visual-C-
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace userguess
{
    internal class car
    {
        int year;
        string make;
        decimal speed;

        public int Year
        {
            get { return year; }
            set { year = value; }
        }
        public string Make
        {
            get { return make; }
            set { make = value; }
        }
        public decimal Speed
        {
            get { return speed; }
            set { speed = value; }
        }

        public car()
        {
            year = Year;
            make = Make;
            speed = 0m;

        }
        
        public void displayinitial()
        {
            MessageBox.Show("Name: " + year.ToString() + ".\nMake: " + make
                + "\nSpeed: " + speed);
        }

        public void acc()
        {
            speed += 5;
            
        }
        public void brake()
        {
            speed -= 5;
            
        }
        
    }
}
