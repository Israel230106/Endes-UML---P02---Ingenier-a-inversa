# Endes-UML---P02---Ingenier-a-inversa

<img width="1245" height="1294" alt="image" src="https://github.com/user-attachments/assets/e438ad68-6132-4434-b51e-ef162aabfdf4" />

¿Qué tipo de relación existe entre Agenda y Contacto?

Existe agregación entre Contacto y Telefono, ya que en el diagrama UML se representa con un rombo vacío (o--), La multiplicidad indica que una Agenda contiene 0..* Contacto, debido a que la Agenda agrupa contactos, pero los contactos pueden existir independientemente de la agenda

¿Qué tipo de relación existe entre Contacto y Telefono?

Tienen una relación de composición (representado con un rombo negro (*--) en el lado de Contacto) porque Un Contacto puede tener 0..* Telefono y los Telefono no tienen sentido si no pertenecen cada uno a un contacto.

¿Qué tipo de relación existe entre Contacto y Direccion?

Aquí, al igual que entre Contacto y Telefono, hay una relación de composición, ya que la relación es representada con un rombo negro , y Dirección no existe de forma independiente en el modelo UML 

¿Por qué los tipos TipoTelefono y TipoVia se modelan como enumerados?

Porque estos no son objetos, sino valores constantes que evitan errores en la escritura o valores no válidos y mejoran la legibilidad, seguridad y mantenibilidad del código.

¿Qué relaciones del diagrama son asociaciones simples y cuáles podrían interpretarse como agregación o composición?

Asociaciones simples:

· Direccion -- TipoVia
· Telefono -- TipoTelefono
· Dependencias de Main hacia otras clases (Main ..>)

Son asociaciones simples porque Solo indican que una clase usa o conoce a la otra.

- Agregación:

·Agenda o-- Contacto

 Como esta relación agrupa contactos, pero no controla completamente su existencia, esta relación se trataría de una agregación.

-Composición

·Contacto *-- Direccion
·Contacto *-- Telefono

Es relación de composición porque el contacto es el dueño de la dirección y los teléfonos.
