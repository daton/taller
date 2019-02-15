# Taller
## Taller Android
 Copia el codiguito siguiente donde te lo indique el profesor
 
 Primero vas a poner esto hasta arriba, son bibliotecas
 
 ```
 import android.content.Intent;
 import android.view.View;
 ```
 Despues esto en el método correspondiente
 
 ```
  findViewById(R.id.boton).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Intent sendIntent = new Intent();
                sendIntent.setAction(Intent.ACTION_SEND);
                sendIntent.putExtra(Intent.EXTRA_TEXT, "Escribe lo que quieras aqui jeje");
                sendIntent.setType("text/plain");
                sendIntent.setPackage("com.whatsapp");
                startActivity(sendIntent);
            }
        });
     
        

