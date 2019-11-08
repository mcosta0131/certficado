# certficado
Arquivo txt para auxiliar a importar cert para a JVM:

==========================================================================================================================================


certificado
==========
keytool -import -alias tomcat -file certificado.cer -keystore keystore.p12 -storepass password

keytool -importcert -file certificado.cer -alias tomcat -keystore"C:/Program Files (x86)/Java/jre7/lib/security/cacerts"

Senha: password
Senha: changeit

#COMO INSTALAR CERTIFICADO NA JVM
# C:\ambienteDesenv\programas\java\ibm_sdk71
# C:\ambienteDesenv\programas\java\ibm_sdk71\jre\lib\security\cacerts
keytool -export -alias tomcat -keystore keystore.p12 -file certificado.cer
keytool -import -alias tomcat -file certificado.cer -keystore "C:\ambienteDesenv\programas\java\ibm_sdk71\jre\lib\security\cacerts"


keytool -export -alias tomcat -keystore keystore.p12 -file viavarejo.cer
keytool -import -alias tomcat -file viavarejo.cer -keystore "C:\ambienteDesenv\programas\java\ibm_sdk71\jre\lib\security\cacerts"


keytool -import -alias tomcat3 -file viavarejo6.cer -keystore "C:\ambienteDesenv\programas\java\ibm_sdk60\jre\lib\security\cacerts"

keytool -import -alias tomcat -file viavarejo7.cer -keystore "C:\Program Files (x86)\Java\jdk1.7.0_80\jre\lib\security\cacerts"
keytool -import -alias tomcat -file viavarejo7.cer -keystore "C:\Program Files (x86)\Java\jdk1.6.0_45\jre\lib\security\cacerts"
