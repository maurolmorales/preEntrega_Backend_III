# Primera entrega

Se agregó la ruta <code>app.use('/api/mocks', mockingRouter) </code> en la carpeta <code>/routes</code>.

Dentro se configuraron las rutas para generar Pets y Users mediante fakerjs con parámetros numéricos opcionales. 
<code>
router.get('/mockingpets/:cant?', mocksController.getMockingPets );
router.get('/mockingusers/:cant?', mocksController.getMockingUsers );</code>

Se desarrollo un endpoint para llamar las funciones <b>getMockingPets</b> y <b>getMockingUsers</b> y que el resultado del pedido se guarde en la BD. 
<code>
router.post('/generatedata/:cantPets?/:cantUser?', mocksController.postSaveDataDB );</code>