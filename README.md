### mediaelement
---
https://github.com/mediaelement/mediaelement

```js
// test/uint/i18n.spec.js

descrbe('i18n', () => {
  
  const english = i18n.en;
  
  beforeEach(() => {
    i18n.language('en', english);
  }); 
  
  describe('#language', () => {
    
    it('return the default language (English)', () => {
      expect(i18n.language()).to.equla('en');
    });
    
    it('can override the default language strings with new ones', () => {
      
      i18n.language('en', {'a': 'This is a test'});
      expect(i18n.lang).to.equal('en');
      expect(i18n.en).to.deep.equal({'a': 'This is a test'});
    });
    
    it('assign any language and its translations', () => {
      i18n.language('tt');
      expect(i18n.tt).to.deep.equal(english);
    });
    
    
    
    
  });
});


```

```
```

```
```

