# Git��������Լ���VScode�е�ʹ��

[![��ľʿ](https://picx.zhimg.com/v2-fade060a30524a50d420ee8ad087fcf1_l.jpg?source=172ae18b)](https://www.zhihu.com/people/ghowoght)

[��ľʿ](https://www.zhihu.com/people/ghowoght)

һ����û�����

��ע��

156 ����ͬ�˸�����

����������**Git��Github������**��Git�Ǹ��汾���ƵĹ��ߣ����������صĴ��빤�̣������Լ�¼�������ݵı������Github��һ�������й�ƽ̨�����ǿ���ʹ��Git�����ش����ϴ���Github��

**ΪʲôҪѧGit**������˵��Git��һ���汾���ƹ��ߣ������Լ�¼�������ݵı�����������Ƕ���Ŀ�Ĺ�������Ҫ�����µ���;��

- **���뱸��**

��һ���򵥵����ӣ�д��һ���������Ҫ�ټ�һ���¹��ܣ��������¹�����Ҫ�Ժܶ���ļ����иĶ������������������ܺ��֣�����¹����Ǹ��ӣ�Ȼ��ͻ����Ż��˵���һ���汾����ʱ������б��ݻ��ã�û�б��ݵĻ��͵�ctrl+z������Ҫ�����Լ��ļ���ָ���ǰ�İ汾

���ʹ��Git�ͺð��ˣ�ֱ��ʹ��git�л��°汾���߷�֧�Ϳ����ˡ�

��Ȼ�ȱ���һ��ԭʼ���룬Ȼ��������ģ�Ҳ��һ���ܼ�����Ч�ķ��������������¹��ܵ����ӣ�������ռ�õ��ڴ�Խ��Խ�󣬶���ÿ���汾����������ֱ�ۿ������ⲻ�������Ƕ���Ŀ�Ĺ���

- **����Э��**

����Ҫ��һ����Ŀ�������Ŀ���ж�����ܣ����������£����ǲ�����һ������һ�����ܵ��������ǽ����Ŷӷֹ����������ͬ�����У���ʱ�����û��ʹ��Git���а汾���ƣ���ô�ڽ���Щ����ͳ��ʱ������ֺܴ������

- **�Ժ�������Ҫ**

Ŀǰ�ܶ๫˾������Git������Ŀ����ѧ��Git���Ժ�Ĺ������Ǻ��кô���

���Ľ�����Git�Ļ����������̣��Լ���Щ���̶�Ӧ��������ָ�����VScode�����õ�Git���н��ܺ���ʾ

## Git��װ

Git��Windows�Ϻ���Linux�ϵ�ʹ�÷�ʽ�����޲�����Ա����е���ʾ��Ҫ��Windows�Ͻ���

### Windows

��[����](https://link.zhihu.com/?target=https%3A//git-scm.com/downloads)�����������°��Git��Ȼ��һ·Next����

### Ubuntu

```bash
sudo apt-get install git
```

## Git��������

������������ͼ��

![img](https://pic1.zhimg.com/80/v2-cd9ae639fa7ba273ffc3753037629ee0_1440w.webp)

- ������(Workspace)��ƽʱ�����Ŀ����ĵط�
- �ݴ���(Index/Stage)��������ʱ��ŸĶ���Ϣ
- ���زֿ�(Repository)����������ύ�İ汾����
- Զ�ֿ̲�(Remote)���йܴ���ķ��������������Ǿ����õ�Github���Ǹ������й�ƽ̨

git�Ļ��������������£�

1. �ڹ���������ӡ��޸��ļ�
2. ������������Ҫ���а汾������ļ������ݴ���
3. ���ݴ������ļ��ύ��git���زֿ�
4. (**optional**)�����زֿ����͵�Զ�ֿ̲�

Ϊ�˷����Ժ��ѧϰ�͹�����������ֱ��ʹ��GUI������Git�����潫�������Ĺ������̽���һЩ���õ�Git������ָ���Щָ���ǱȽϼ򵥵ģ�������֮��������GUI�汾��Git���൱������

### ��ʼ��

��ʼ��git�������ַ�ʽ��

```bash
# ��ʽһ:��������һ��git
git init
# ��ʽ��:��Զ�˿�¡һ���ֿ�
git clone https://gitee.com/xxxxxx/xx.git
```

��������

```bash
# �����û���
git config --global user.name "name"
# ��������
git config --global user.email "name@mail.com"
```

ɾ��Զ�ֿ̲�

```bash
git remote rm origin
```

���Զ�ֿ̲�

```bash
git remote add origin https://gitee.com/xxxxxx/xx.git
```

### ������Զ�ֿ̲�

�����޸��ļ�������ݴ���

```bash
git add dir/filename # ���ָ���ļ�
git add . # ����������޸��ļ�
```

���ݴ����ĸĶ��ύ�����صİ汾�⣬ʹ��`git commit`�������Ǿͻ��ڱ��ذ汾������һ��40λ�Ĺ�ϣֵ�����ڰ汾����

```bash
git commit -m "message" # message���Ǳ����ύ�ļ�Ҫ˵��
```

�����ϴ���ע��������ǰ��Ҫ�ȴ�Զ����ȡ

```bash
git push -u origin master # master���Ը���Ϊ������֧
```

### ��Զ�ֿ̲���ȡ

���±��أ�

```bash
git pull origin master # master���Ը���Ϊ������֧
```

### ��֧����

��֧�����ǰ汾������һ������Ҫ�����ݣ���Git����Ҫ���л�/������֧(checkout)���ϲ���֧(merge)����ָ��

�����ǲ��ַ�֧������ָ���ͼʾ��ԲȦ���ʾһ���ύ(commit)��¼�����α�ʾ��֧����ָ��һ���ύ��¼���������¼���Ա���֮ǰ���е��ύ��¼

���ȳ�ʼ����һ��git�����git��ֻ��һ��`master`��֧����������commit��¼

![img](https://pic1.zhimg.com/80/v2-e4f88ddafff72af14821b1f014280134_1440w.webp)

�������Ǵ���һ���·�֧������Ϊ`develop`��

```bash
git checkout -b develop # ��ʾ�������л���develop��֧
```

![img](https://pic4.zhimg.com/80/v2-d5504a1b7cdc368a01b900f013084527_1440w.webp)

��ʱ`master`��֧��`develop`��֧��ָ��C1����ύ��¼�����Ƿֱ�����������֧�Ͻ����޸Ĳ��ύ��

```bash
git commit
git checkout master # �л���master��֧
git commit
```

![img](https://pic1.zhimg.com/80/v2-afdb0ab985d5784b4e063938963ca970_1440w.webp)

���Կ���`master`��֧��`develop`��ָ֧���˲�ͬ���ύ��¼�����������ǽ�`develop`��֧�ϲ���`master`��֧��

```bash
git merge develop
```

![img](https://pic2.zhimg.com/80/v2-991bc8e3e03d37d6d148df5981090bad_1440w.webp)

ִ�������ָ��󣬲�����һ���µ��ύ��¼C4����C4���ǿ��Ա���֮ǰ���е��ύ��¼�����Ǵ�ʱ`master`��֧��`develop`��֧��Ȼָ��ͬ���ύ��¼�������л���`develop`��֧����`master`��֧�ϲ���`develop`��֧�У�

```bash
git checkout develop
git merge master
```

![img](https://pic3.zhimg.com/80/v2-c9489a4cc8cf75238823b852a743a5c2_1440w.webp)

### ���ǩ

ʹ��Git���Ը�ָ���ύ���ϱ�ǩ������ͻ����ʾ����ύ�����罫�ύ���Ϊv1.0��v2.0���ȵ�

- **�оٱ�ǩ**

ʹ������������г����б�ǩ

```bash
git tag
```

����ǩ̫��ʱ������ʹ������ָ���г�����ָ���ַ��ı�ǩ

```bash
git tag -l "v1.*"
```

- **������ǩ**

���-aѡ��ɴ�����ǩ�����£�

```bash
git tag -a v1.0 -m "version 1.0"
```

���������Ϊ��ǰ�ύ����һ����ǩ����ǩ��Ϊv1.0��-mѡ�����Ǹñ�ǩ�ĸ�ע��Ϣ

- **���ͱ�ǩ**

ֻʹ��git push������Ĭ������²��Ὣ��ǩ���͵� Զ�ֿ̲⣬�ڴ�����ǩ����Ҫִ���������ָ����ǩ���͵�Զ�ֿ̲⣺

```bash
git push origin <tagname>
```

���Ҫ���Ͷ���±�ǩ������ʹ��git push��--tagsѡ����б�ǩ���͵�Զ�ֿ̲⣺

```bash
git push origin --tags
```

- **ɾ����ǩ**

ʹ��git tag��-dѡ���ɾ�����زֿ��ϵ�ָ����ǩ�����£�

```bash
git tag -d <tagname>
```

���Ǹ�ָ���ɾ��Զ�ֿ̲��еı�ǩ ������Ҫʹ����������������Զ�ֿ̲⣺

```bash
git push remote :refs/tags/<tagname>
```

- **�л���ǩ**

ʹ��git checkout <tagname>ָ��ɽ�git�ֿ��HEADָ��ָ���ǩ���ڵ��ύ�����£�

```bash
git checkout v1.0
```

## VScode�е�Gitʹ��

### ���زֿ����

���Բֿ��Ѿ������ٵ��ļ������޸ĵ�ʱ�򣬻��������ļ�״̬����ͼ��

![img](https://pic3.zhimg.com/80/v2-ef4f2f4e1453c1311cf6ffb0f045057a_1440w.webp)

- M(Modify)����ʾ���ļ������޸�
- D(Delete)����ʾ���ļ���ɾ��
- U(Update)����ʾ���ļ�������ӵ�

ѡ���ļ����ɲ鿴�ѽ��е��޸�

![img](https://pic1.zhimg.com/80/v2-21bd732c279178de83fa5d46fd6092a4_1440w.webp)

���������Զ���Щ���Ľ��д�������ѡ������޸Ļ��߱����޸ģ�ѡ������޸ĵĻ������ļ��ͻ���˵��ϴα���İ汾

![img](https://pic4.zhimg.com/80/v2-cf629edd3ff909f59eb01649d91caf6b_1440w.webp)

Ҳ���Ե�������ͼ������и��Ľ��д���

![img](https://pic1.zhimg.com/80/v2-99bad335d95735ca5b3bdcbd411bff30_1440w.webp)

����ѡ�񱣴������޸ģ��������޸��ļ��ͻᱣ�浽�ݴ�������Ӧ��git����Ϊ`git add .`

���������ݴ����ĸĶ��ύ�����صİ汾�⣬����Ϸ��ġ��̡�����Ӧgit����`git commit`��Ȼ�����message����

![img](https://pic2.zhimg.com/80/v2-e0396dff6e22c3363f64a7f640233455_1440w.webp)

��ʱ�����е��޸ľ��Ѿ����������

![img](https://pic2.zhimg.com/80/v2-557dcf3b8c86daa348daa9fca6f8c5d1_1440w.webp)

### ���͵�Զ�ֿ̲�

�����زֿ��ϵ��޸����͵�Զ�ֿ̲⣬��Ӧgit����`git push`

![img](https://pic3.zhimg.com/80/v2-7f0d54b382afc8f6059c83de4d7c7022_1440w.webp)

һ������£�VScode�ᵯ���˺���������봰�ڽ��е�¼

���鿴Զ�ֿ̲⣺

![img](https://pic2.zhimg.com/80/v2-760189c2e52dbdcd29962717d0270561_1440w.webp)

### ��Զ�ֿ̲���ȡ

���������ƣ���ͼ����Ӧgit����`git pull`

![img](https://pic1.zhimg.com/80/v2-5742bd638076376dea0eeea548850f34_1440w.webp)

### ��֧����

VScode����ֱ�������½Ǵ���/�л���

![img](https://pic3.zhimg.com/80/v2-675d844f01c011c1a0a422379dd42f6e_1440w.webp)

�ϲ���֧

![img](https://pic3.zhimg.com/80/v2-9447b8ffaeca8879a8c819f7834c1ec2_1440w.webp)

������ϲ��ķ�֧�ϵ��޸ĺ�masterû�г�ͻ���Ϳ���ֱ�Ӻϲ��������ڶ���Э��ʱ���������������֧���ڲ�ͬ�޸ĵ��������ʱ���Ҫ����Щ��ͻ���д���

![img](https://pic3.zhimg.com/80/v2-98ef03a3554f080504c3f125179d3306_1440w.webp)

### GitLens���

ʹ��VScode�Դ���git֧�ֶ��ڸ��˿�����˵�Ѿ��㹻�ˣ�������Ӧ���Ŷ�Э��ʱ���ļ���ͻʱ�����Բ��㣬��ʱ�����ǿ��Խ���VScode�е�GitLens�����ʹ�÷������[gitԴ���������GitLens](https://link.zhihu.com/?target=https%3A//www.jianshu.com/p/a91cb8a2e55d)

## �ο�

[Git ��֧�������ʵ��developer.ibm.com/zh/articles/j-lo-git-mange/](https://link.zhihu.com/?target=https%3A//developer.ibm.com/zh/articles/j-lo-git-mange/)

[Git�̳�www.liaoxuefeng.com/wiki/896043488029600![img](https://pic3.zhimg.com/v2-23dad9e5cdf40848a5ad1c72bf5de2c6_180x120.jpg)](https://link.zhihu.com/?target=https%3A//www.liaoxuefeng.com/wiki/896043488029600)

[VScode ���git��ȫ��ʹ�����̣���Ҳ���ü�סgit�������ˣ�blog.csdn.net/weixin_43314519/article/details/107572206![img](https://pic3.zhimg.com/v2-ee64702a944d84466a59ea45c2f45e2a_ipico.jpg)](https://link.zhihu.com/?target=https%3A//blog.csdn.net/weixin_43314519/article/details/107572206)

[Learn Git Branchingoschina.gitee.io/learn-git-branching/![img](https://pic1.zhimg.com/v2-8e7132076f76bc1c65eb1f41d15e1aa8_180x120.jpg)](https://link.zhihu.com/?target=https%3A//oschina.gitee.io/learn-git-branching/)



�༭�� 2022-02-02 15:18