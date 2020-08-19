# backend-agenda
  Eu este projeto no canal do Youtube da Michelli Brito.
  Acrescentei alguns metódos e um atributo nas pastas(document,repository,service e controller) que são:
   - No document na class LiveDocument coloquei um atributo chamado categoria;
   - No repository interface adcionei um metódo chamado de: List<LiveDocument> findByCategoria(String categoria);
   - No service foi esse metódo: 
      - public List<LiveDocument> findByCategoria(String categoria);
      - E fiz um sobrecarga nesse metódo: public List<LiveDocument> findAll() ;
   - No controller foram esses metodos:
       - public ResponseEntity<List<LiveDocument>> getCategoria(@PathVariable(value="categoria") String categoria);
       - public ResponseEntity<List<LiveDocument>> findAll();
       - no metódo public ResponseEntity<LiveDocument> updateLive(@PathVariable(value="id") String id,
                                                      @RequestBody @Valid LiveDocument liveDocument),
          coloquei o liveDocument.setRegistrationDate(LocalDateTime.now());
        
    Coloquei o driver do mongodb local. 
