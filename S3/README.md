# Primero se ejecuta este comando en la terminal para agregar variable de ambiente:

mybucket=$(aws s3api list-buckets --output text --query 'Buckets[?contains(Name, `notes-bucket`) == `true`].Name')

# Ejecutar en la terminal el siguiente comando para validar la variable:
mybucket=$(aws s3api list-buckets --output text --query 'Buckets[?contains(Name, `notes-bucket`) == `true`].Name')