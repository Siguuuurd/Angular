���L��[�C�P�ĂȂ��R�[�h - Web�G���W�j�A�̃u���O](https://wp.tech-style.info/archives/683)�����p  
��REST API�Ƃ�  
�EHTTP�̋Z�p���ő�����p����A�V���v���Ȑ݌v���@  
�E�u���̃��\�[�X���v�u�ǂ̂悤�Ɂv���삷�邩��URI��HTTP���\�b�h�ŕ\������  
�E���\�[�X�w���̐݌v  
�E�Z�b�V�����ȂǏ�Ԃ��Ǘ������A�K�����̃��N�G�X�g�ŏ�������������  



���L��[REST���� ��b�m��](https://qiita.com/TakahiRoyte/items/949f4e88caecb02119aa)�����p  
��REST�Ƃ�  
REST(REpresentational State Transfer)��Web�T�[�r�X�̐݌v���f���ł��B  
REST��Web�T�[�r�X�́A���̃T�[�r�X��URI��HTTP���\�b�h�ŃA�N�Z�X���邱�ƂŃf�[�^�̑���M���s���܂��B  

��REST�̐݌v�����ł���RESTful  
REST�͐݌v�ɍۂ��ȉ���݌v�����Ƃ���悤�񌾂���Ă��܂��B  

�E�A�h���X�w��\��URI�Ō��J����Ă��邱��  
�@��j
�@https://test.com/SampleList/Test/1  
�@
�@�uSampleList�v��MVC�̃R���g���[���[�ɓ�����B  
�@C#�ł́uSampleListController�v�ƃR���g���[�����ɂȂ�B  
�@
�@�uSampleList�v�̒��́uTest�v���w�肷��B(�P����GET�Ȃǂ���ꍇ�͕s�v�B)  
�@URL�́u1�v�̓p�����[�^�B
�@C#�ł�[HttpGet("Test/{no?}")]�ƋL�ڂ���B�u?�v��NULL��������BNULL�������Ȃ��ꍇ�́u?�v�͕s�v�B  

�E�C���^�[�t�F�[�X(HTTP���\�b�h�̗��p)�̓��ꂪ����Ă��邱��  
�@REST�ŗp������HTTP���\�b�h�͉��L�̂悤�ɑΉ��t�����܂��B  
�@�擾�FGET  
�@�o�^�FPOST  
�@�X�V�FPUT  
�@�폜�FDELETE  
�@
�E�X�e�[�g���X�ł��邱��  
 �X�e�[�g�Ƃ́u��ԁv���Ӗ����܂��B����ăX�e�[�g���X�́u��Ԃ��Ȃ��v�Ƃ����Ӗ��ɂȂ�܂��B  
 �X�e�[�g���X�Ȃ����ɂ����ăT�[�o�[�̓N���C�A���g�̃Z�b�V��������ێ����܂���B  
 �t�ɃX�e�[�g�t���Ȃ����ɂ����Ă̓Z�b�V������񂪕ێ�����܂��B  
 ���ꂾ���ł͗������Â炢���Ƃ�����Ǝv���̂ŁA���L�u���O�̋q�ƓX���̉�b�̗��ǂ�ł݂Ă��������B  
[yohei-y:weblog](http://yohei-y.blogspot.com/2007/10/blog-post.html)  


�E�������ʂ�HTTP�X�e�[�^�X�R�[�h�Œʒm����邱��  
�X�e�[�^�X�R�[�h��Web�T�[�o�[����̃��X�|���X��\���R�[�h�ł��B  
REST��HTTP���\�b�h�𗘗p���Ă���̂�HTTP�X�e�[�^�X�R�[�h�����̌��ʂƂ��ĕԋp����͎̂��R�ȗ���ł��B  
�ȉ��ɕp�o����HTTP�X�e�[�^�X�R�[�h���܂Ƃ߂܂��B  

### HTTP�X�e�[�^�X�R�[�h�ꗗ

|�R�[�h  | ���                  |    ����                                                 |
|:------:| --------------------- | ------------------------------------------------------- |
| 200    | OK                    | �N�G�X�g������ɏ������ꂽ                              |
| 201    | Created               | ���N�G�X�g������ɏ�������A�V�K���\�[�X���쐬���ꂽ    |
| 400    | No Content            | ���N�G�X�g������ɏ������ꂽ���A�Ԃ��V�K���͂Ȃ�      |
| 401    | Bad Request           | �T�[�o�[�������ł��Ȃ������ȗv���ł���                  |
| 403    | Unauthorized          | �v�����ꂽ���\�[�X�ɂ͔F�؂��K�v�ł���                  |
| 404    | Forbidden             | �v�����ꂽ���N�G�X�g�͋��ۂ��ꂽ                        |
| 405    | Not Found             | �v�����ꂽ���\�[�X�̓T�[�o�[�ɑ��݂��Ȃ�                |
| 500    | Internal Server Error | �T�[�o�[�ŃG���[����������                              |

