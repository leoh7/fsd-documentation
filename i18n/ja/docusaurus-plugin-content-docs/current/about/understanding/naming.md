---
sidebar_position: 4
---

# ネーミング

異なる開発者は異なる経験と背景を持っているため、同じエンティティが異なる名前で呼ばれることによって、チーム内で誤解が生じる可能性があります。例えば

- 表示用のコンポーネントは「ui」、「components」、「ui-kit」、「views」などと呼ばれることがある。
- アプリケーション全体で再利用されるコードは「core」、「shared」、「app」などと呼ばれることがある。
- ビジネスロジックのコードは「store」、「model」、「state」などと呼ばれることがある。

## Feature-Sliced Designにおけるネーミング {#naming-in-fsd}

FSD設計方法論では、以下のような特定の用語が使用されます。

- 「app」、「process」、「page」、「feature」、「entity」、「shared」といった層の名前、
- 「ui」、「model」、「lib」、「api」、「config」といったセグメントの名前。

これらの用語を遵守することは、チームメンバーやプロジェクトに新しく参加する開発者の混乱を防ぐために非常に重要です。標準的な名称を使用することは、コミュニティに助けを求める際にも役立ちます。

## 名前衝突 {#when-can-naming-interfere}

名前衝突は、FSD設計方法論で使用される用語がビジネスで使用される用語と重なっている場合に発生する可能性があります。例えば

- `FSD#process`と、アプリケーション内でモデル化されたプロセス、
- `FSD#page`と、マガジンのページ、
- `FSD#model`と、自動車モデル。

開発者がコード内で「プロセス」という言葉を見た場合、どのプロセスが指されているのかを理解するのに余分な時間を費やすことになってしまいます。このような**衝突は開発プロセスを妨げる場合があります**。

プロジェクトの用語集にFSD特有の用語が含まれている場合、これらの用語をチームや技術的に関心のない関係者と議論する際には特に注意が必要です。

チームとの効果的なコミュニケーションのためには、用語の前に「FSD」という略語を付けることをお勧めします。例えば、プロセスについて話すときは、「このプロセスをFSDのフィーチャー層に置くことができる」と言うことができます。

逆に、技術的でない関係者とのコミュニケーションでは、FSDの用語の使用を制限し、コードベースの内部構造に言及しない方が良いでしょう。