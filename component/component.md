//クラス（モジュール）をインポートする  
import { NgModule } from '@angular/core';  
import { SampleListService } from './sample-list.service';  
import { AppComponent } from './app.component';  

// @NgModuleデコレータ（NgModule メタデータ）  
@NgModule({  
    imports: [FormsModule],  
    declarations: [SampleComponent],  
    providers: [SampleService],  
    bootstrap: [SampleComponent]  
})

■NgModuleについて  
[モジュールのイントロダクション](https://angular.jp/guide/architecture-modules)  
[属性ディレクティブ]()  

 メモ：@NgModuleに記載する場合、必要なものだけでも動作するため、すべて定義する必要はない。  


//  
@Component({  
    selector: 'app-sample-senteihyo',  
    templateUrl: './sample-senteihyo.component.html',  
    styleUrls: ['./sample-senteihyo.component.css'],  
    providers: [SampleListService]  
})


//最初に呼び出される  
export class SampleComponent implements OnInit {  
// ページ内の変数定義  
private no: Number;  
private name: string[] = [];  
private data; any = null;  

//
//@ViewChild  

    constructor(
        private datePipe: DatePipe,  
        private sampleListService: SampleListService,

    ) {  
    }  

    /**
     * 初期処理  
     */
    ngOnInit() {  
    }  

    /**
     * 終了処理
     */
    ngOnDestroy() {  
        }  
    }  
 
}    