Valores Aleatorios
==================
 > Significa: Valores (Pseudo) Impredecibles
 > Procedimiento:
   - Definir/Iniciar Sistema Aleatorio ( 1 Vez )
     public static final Random RND = new Random();
   - Utilizar sistema Aleatorio ( N Veces )
 > Tipos de Datos: Primitivos - Métodos Específicos
   - Enteros - nextInt/nextLong
     int valor = RND.nextInt();                    // [Integer.MIN.VALUE .. Integer.MAX_VALUE]
     int valor = RND.nextInt(MAX - MIN + 1) + MIN; // [MIN .. MAX]
   - Reales - nextFloat/nextDouble
     double valor = RND.nextDouble();              // [0.0 .. 1.0[
     double valor = RND.nextDouble() * (MAX - MIN) + MIN; // [MIN .. MAX[
   - Lógicos - nextBoolean()
     boolean valor = RND.nextBoolean();            // true/false
   - Caracteres
     char valor = (char)(RND.nextInt(CAR_MAX - CAR_MIN + 1) + CAR_MIN); // [CAR_MIN .. CAR_MAX]
