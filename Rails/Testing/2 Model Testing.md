1. Generate for model we want to test 
2.  `rails g rspec:model article`
3. Add `faker` gem in Gemfile *(optional)*
4. Not fill the dummy data in `factories/model_name.rb` file
```rb
FactoryBot.define do
  factory :article do
    title { Faker::Book.title }
    body { Faker::Book.genre }
  end
end
```
5. In model_spec file write the testcase like this

```rb
require 'rails_helper'

RSpec.describe Article, type: :model do
  context 'when creating an article' do
    # It will create a new method named article which when called return article object
    let(:article) { build :article }

    # logic we want to perform
    it 'should be valid user with all attributes' do
      expect(article.valid?).to eq(true)
    end
  end
end
```

TO create a article with nil `body`
```rb
let(:article) { create :article, body : nil }
```

- To run a testcase depending on the line number we can write.
- `rspec spec/models/article_spec.rb:12` <- Line number
