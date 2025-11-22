<H1>Instrucciones de instalación</H1>
・Descarga el zip y abrelo en Visual studio 

<br><br><br><br>


<H1>Capturas de pantalla de la aplicación funcionando</H1>
<img width="916" height="455" alt="image" src="https://github.com/user-attachments/assets/26f567c9-f9f6-4ce4-80e4-374f712617de" />
<img width="908" height="456" alt="image" src="https://github.com/user-attachments/assets/cc7cc6e6-dcb3-472a-82ce-6584939c3071" />
<br>
<H3>Nota guardada</H3>
<img width="913" height="464" alt="image" src="https://github.com/user-attachments/assets/f6c277ff-7451-4819-9471-143a633826db" />
<br>
<H3>Nota eliminada</H3>
<img width="915" height="467" alt="image" src="https://github.com/user-attachments/assets/ae5dc9ff-11f6-4ce5-be0b-4c2739667dd7" />
<br>
<H3>Nota modificada</H3> (Se modifico el titulo)
<img width="915" height="464" alt="image" src="https://github.com/user-attachments/assets/312b2357-55c8-448d-94f4-aaf26226f234" />
<br>
<H3>Busqueda por Tag</H3>
<img width="917" height="464" alt="image" src="https://github.com/user-attachments/assets/a1f71496-1f53-4608-af8f-327c7ecbf127" />
<img width="912" height="463" alt="image" src="https://github.com/user-attachments/assets/fe9486c8-cd4c-4a5c-9d65-7a1579f13943" />
<br>
<H3>Recargar</H3>
<img width="916" height="463" alt="image" src="https://github.com/user-attachments/assets/b8057df2-d69e-408f-b3f1-eda849bf1b08" />


<br><br><br><br>
<H1>Ejemplo de configuración de la cadena de conexión a MongoDB</H1>
<Code>


              try
            {
                var client = new MongoClient("mongodb://localhost:』』』』』");
                var bdd = client.GetDatabase("NotesBDD");
                var notesCollection = bdd.GetCollection<Nota>("Notes");
                MessageBox.Show("Conectado");
                return notesCollection;
            }
            catch (MongoException e)
            {
                MessageBox.Show("No se conecto");
                return null;
            }

</Code>
