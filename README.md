import java.util.ArrayList;
public class EventOrganiser {

        private String CustId;
        private String CustName;
        private String CustAddr;


        public String getCustId() {
            return CustId;
        }

        public void setCustId(String custId) {
            CustId = custId;
        }

        public String getCustName() {
            return CustName;
        }

        public void setCustName(String custName) {
            CustName = custName;
        }

        public String getCustAddr() {
            return CustAddr;
        }

        public void setCustAddr(String custAddr) {
            CustAddr = custAddr;
        }

        public String getCustEmail() {
            return CustEmail;
        }

        public void setCustEmail(String custEmail) {
            CustEmail = custEmail;
        }

        public int getCustPhone() {
            return CustPhone;
        }

        public void setCustPhone(int custPhone) {
            CustPhone = custPhone;
        }

        private String CustEmail;
        private int CustPhone;

        public static void PrintGuest() {
            ArrayList<String> guest = new ArrayList<String>();
            guest.add("Denny Caknan");
            guest.add("BlackPink");
            System.out.println("Spesial Guest " + guest);
            System.out.println();

            System.out.println("=========================");
            System.out.println("Daftar Nama Tamu Undangan");
            System.out.println("=========================");


            String[] Tamu = new String[10];
            for (int index = 0; index < Tamu.length; index++) {
                System.out.println("Nama Tamu " + (index + 1) + " : " + Tamu[index]);
                EventOrganiser Namatamu = new EventOrganiser();
                ArrayList<EventOrganiser> DaftarTamu = new ArrayList<EventOrganiser>();
                for (EventOrganiser tamu : DaftarTamu) {
                    System.out.println("User Id     : " + tamu.getCustId());
                    System.out.println("Nama Tamu   : " + tamu.getCustName());
                    System.out.println("Alamat      : " + tamu.getCustAddr());
                    System.out.println("Email       : " + tamu.getCustEmail());
                    System.out.println("No.Hp       : " + tamu.getCustPhone());
                }
            }
        }
        public void CetakNamaTamuUndangan(){
            System.out.println("User Id     : " + this.getCustId());
            System.out.println("Nama Tamu   : " + this.getCustName());
            System.out.println("Alamat      : " + this.getCustAddr());
            System.out.println("Email       : " + this.getCustEmail());
            System.out.println("No.Hp       : " + this.getCustPhone());
        }

        public EventOrganiser(){

        }

        public EventOrganiser(String custid,String custname, String custaddr, String custemail, int custphone){
            this.CustId = custid;
            this.CustName = custname;
            this.CustAddr = custaddr;
            this.CustEmail = custemail;
            this.CustPhone = custphone;
        }
    }
