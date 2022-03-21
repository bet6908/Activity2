# Activity2
# Convert to Mars Weight
# link to video of application [https://screencast-o-matic.com/watch/c3e2nkVFuDr]

namespace MarsWeigth
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void btn_convertWgt_Click(object sender, EventArgs e)
        {
            double marsGravity = 2.65251989;
            double earthWgt;
            double marsWgt;

            earthWgt = double.Parse(txtWgtEarth.Text);
            marsWgt = earthWgt / marsGravity;


            txtOutput.Text = marsWgt.ToString();

        }
    }
}
