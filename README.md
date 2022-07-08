# -guru
private void submitActionPerformed(java.awt.event.ActionEvent evt) {                                       
        details s = new details();
        s.name = txtName.getText();
        s.fName = fatherName.getText();
        s.address = address.getText();
        s.phoneNo = JLable3.getText();
        if(male.isSelected())
        {
            s.gender = "Male";
        }
        else if(female.isSelected())
        {
            s.gender = "Female";
        }
        else
        {
            s.gender = "Other";
        }
        s.district = jLabel6.getText();
        s.taluk = jLabel7.getText();
        s.nativePlace = jLabel8.getText();
        s.previousCollage = jLabel9.getText();
        s.percentage = jLabel9.getText();
        if(pass.isSelected())
        {
            s.result = "Pass";
        }
        else 
        {
            s.result = "Fail";
        }
        printDetails sc = new printDetails(s);
        sc.setVisible(true);
        s.setVisible(false);
    }                                      

    private void clearActionPerformed(java.awt.event.ActionEvent evt) {                                      
        txtName.setText("");
        fatherName.setText("");
        jTextArea1.setText("");
        JLable3.setText("");
        male.setText("");
        female.setText("");
        other.setText("");
        jLabel6.setText("");
        jLabel7.setText("");
        jLabel8.setText("");
        jLabel9.setText("");
        pass.setText("");
        fail.setText("");
    }                                     

    /**
     * @param args the command line arguments
     */
    public static void main(String args[]) {
        /* Set the Nimbus look and feel */
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
         * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
         */
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(DetailsForm.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(DetailsForm.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(DetailsForm.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(DetailsForm.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new DetailsForm().setVisible(true);
            }
        });
    
    Capture](https://user-images.githubusercontent.com/108912308/177906997-3f1f1e00-3a8f-4cf4-8b4e-521ca2ca485a.PNG)
![Uploading Capture.PNG…]()
