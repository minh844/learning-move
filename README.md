# learning-move

aptos account fund --profile local --account local

aptos account create-resource-account --profile local --seed 1



aptos move publish --profile local


aptos move run --profile local \
  --function-id 'fe634c330d389f6445c1cbfefc272e5820c68d232e436b07f10dc2bc01723f47::halo_coin::register'


aptos move run --profile local \
  --function-id 'fe634c330d389f6445c1cbfefc272e5820c68d232e436b07f10dc2bc01723f47::halo_coin::mint_me' \
  --args 'u64:20000000'


aptos move run --profile local \
  --function-id 'fe634c330d389f6445c1cbfefc272e5820c68d232e436b07f10dc2bc01723f47::fanv4token::init_fanv4'

aptos move run --profile local \
  --function-id 'fe634c330d389f6445c1cbfefc272e5820c68d232e436b07f10dc2bc01723f47::fanv4token::register'

aptos move run --profile local \
  --function-id 'fe634c330d389f6445c1cbfefc272e5820c68d232e436b07f10dc2bc01723f47::fanv4token::mint' \
  --type-args '0xfe634c330d389f6445c1cbfefc272e5820c68d232e436b07f10dc2bc01723f47::fanv4token::FANV4' \
  --args address:fe634c330d389f6445c1cbfefc272e5820c68d232e436b07f10dc2bc01723f47 u64:5000000000000000000

